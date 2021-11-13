<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redmine`

-	[`redmine:4`](#redmine4)
-	[`redmine:4-alpine`](#redmine4-alpine)
-	[`redmine:4-passenger`](#redmine4-passenger)
-	[`redmine:4.0`](#redmine40)
-	[`redmine:4.0-alpine`](#redmine40-alpine)
-	[`redmine:4.0-passenger`](#redmine40-passenger)
-	[`redmine:4.0.9`](#redmine409)
-	[`redmine:4.0.9-alpine`](#redmine409-alpine)
-	[`redmine:4.0.9-passenger`](#redmine409-passenger)
-	[`redmine:4.1`](#redmine41)
-	[`redmine:4.1-alpine`](#redmine41-alpine)
-	[`redmine:4.1-passenger`](#redmine41-passenger)
-	[`redmine:4.1.5`](#redmine415)
-	[`redmine:4.1.5-alpine`](#redmine415-alpine)
-	[`redmine:4.1.5-passenger`](#redmine415-passenger)
-	[`redmine:4.2`](#redmine42)
-	[`redmine:4.2-alpine`](#redmine42-alpine)
-	[`redmine:4.2-passenger`](#redmine42-passenger)
-	[`redmine:4.2.3`](#redmine423)
-	[`redmine:4.2.3-alpine`](#redmine423-alpine)
-	[`redmine:4.2.3-passenger`](#redmine423-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:4`

```console
$ docker pull redmine@sha256:75c11d669206fefdb4e833f087be5a76327fe402ebda35ac41880656cf9c2128
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

### `redmine:4` - linux; amd64

```console
$ docker pull redmine@sha256:23da6bbd8146ba5ebc6c565af6a4941d0a836fb5f2b3cf8281d954a84047c675
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195500650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777ff92e6fdbdb00a6ebcf1c2df29c52c4cbb171e418bcee49451b9df8ddf3b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:08f124ad97cbf3d78e62b390897fbd0a6e47f4901f4ce4f632d68de47d1236c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196991904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750dc7fdc53efaea0a675c5102c8cc3d6c8e5fb47e2bb056eae33416edf86f72`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 07:03:18 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 07:07:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:07:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:07:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:07:39 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:06:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:06:17 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:06:19 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:06:20 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:06:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:06:24 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:06:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:06:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:13:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:13:17 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:13:19 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:13:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:13:22 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854afe8d48105a800902d829046a9890cab76441d450aa59877c28405734daed`  
		Last Modified: Tue, 12 Oct 2021 07:33:59 GMT  
		Size: 13.9 MB (13871429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97d908af060f6e00c4e7a607087a50b553e21e08c6a8c70274a3d81ea0b3ef`  
		Last Modified: Tue, 12 Oct 2021 07:33:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a08bb1308b5863e00403e1a34c4cb2a9aafa57091f2d1faa4936463e4f8de79`  
		Last Modified: Wed, 13 Oct 2021 03:32:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b177e5e016cce70192ebf1277d5a21559c74cf5aa60e6bff5dfb31a9d5767e8`  
		Last Modified: Wed, 13 Oct 2021 03:32:45 GMT  
		Size: 89.6 MB (89577077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa429c867c2a22535e2c33e168d8de14f69c6f13124dc7494d06630528d03c43`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168fe406bb1360b18d49546d4af05cccf7fb548d99e4f4663d83dab19f23f4be`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2ee921f4dfd9c1a73cfe3b44b39e67f1af385494dd03e3fe1cbdc9c31aaf1`  
		Last Modified: Wed, 13 Oct 2021 03:32:04 GMT  
		Size: 3.1 MB (3063249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892b495be3664dd078f8510b6b3222fec0b0eeceaaa8fcc540d7ced595ecf23`  
		Last Modified: Wed, 13 Oct 2021 03:32:21 GMT  
		Size: 55.3 MB (55253893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea12a2e245bbbc4585eb36f1a1709b9035c2beaac9e1be72d14f2bf9c84118e`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:900b0cad4acc6dc28f8f9e3279e4a10121c4d247bd540f66d7ff40fcdf914200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190138732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88b04a543401c43e354aa169b439ad085b11a2b6acbde3b9a6a36f4307bec08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 03:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:10:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:10:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:10:57 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:34:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:35:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:35:44 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:35:45 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:35:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:35:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:35:48 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 06:35:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 06:35:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:41:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:41:11 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:41:12 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:41:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ab36f90d94f50bb2f0b4be72799049691d9d0f05aadbe4e5cba89a3989efd1`  
		Last Modified: Tue, 12 Oct 2021 03:41:56 GMT  
		Size: 13.8 MB (13767235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a22941e2b0ce8584f2fa791a8370a30bd3a202fa73a1dd64d00a85bf075916a`  
		Last Modified: Tue, 12 Oct 2021 03:41:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6828dc1bb7b47f9d60169ee81885096702049306577ce953096d5057c12e91af`  
		Last Modified: Wed, 13 Oct 2021 06:55:56 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e9962d77928a7fea0f4dd24c838a24f72da3eba59ed75e59a3557633655398`  
		Last Modified: Wed, 13 Oct 2021 06:56:52 GMT  
		Size: 85.6 MB (85590281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894593e78f4567729a26e4302a660a56ee7289a18398fb9ec5b526be2466b739`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f705a0b143059f649ff99fd7d343002386794bfe675456f393697b71d9dbc5`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14825a50627a0f65eec1cc695fb3896ea4d8a22a09fc112bc902fcbbdd53be02`  
		Last Modified: Wed, 13 Oct 2021 06:56:03 GMT  
		Size: 3.1 MB (3063246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461661b0c3351479c43855bab9a39d5482ee87a52376bc2898c48b83ce9ada1`  
		Last Modified: Wed, 13 Oct 2021 06:56:20 GMT  
		Size: 55.1 MB (55101134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b2c0757c967dd445d6615d9fa9fcaac7b289a198fbad58001af82cc9edbbc8`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e7d61bc03c6ee6237c30fc72d8e78f9ae68806cc5a2cf46b7656b4b20eee7fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202799730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d1150fcdbed35bf916de083686b185418c1e6a6899a3b61c1b50d0803144fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:27:15 GMT
ENV RUBY_MAJOR=2.7
# Wed, 13 Oct 2021 17:27:16 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 13 Oct 2021 17:27:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 13 Oct 2021 17:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:28:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:28:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:28:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:07:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:07:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:07:32 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:07:33 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:07:34 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:07:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:07:36 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 18:07:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 18:07:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:10:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:10:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:10:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:10:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:10:14 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:10:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e838a1f60b724d27421dc669bb812af64671ae1601d8730a909695f985a9853`  
		Last Modified: Wed, 13 Oct 2021 17:49:43 GMT  
		Size: 14.1 MB (14143875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963345e088e83677ac3681509027812db0797dd4e631453708af27bbb7645249`  
		Last Modified: Wed, 13 Oct 2021 17:49:41 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394c6771c31ed3bd4fb7c995c8386bec3486e771e2dfa0681f7c5ea822bb971`  
		Last Modified: Wed, 13 Oct 2021 18:16:19 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da764cc87fa4bae907bda083490a29da7979cadd80814f5f362363a376593464`  
		Last Modified: Wed, 13 Oct 2021 18:16:50 GMT  
		Size: 92.6 MB (92615308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3a357444ace950e06fd5b35b20936a1a04a878a138b079900a2a4e02d62a3`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291526f865480d0636e29e2568a193613d43500bc8436edc5155cba7be88cae5`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276061b01ba9d6d30524f2fe777d3cec8be623bcfe6dab6b1c508872ddda38a9`  
		Last Modified: Wed, 13 Oct 2021 18:16:18 GMT  
		Size: 3.1 MB (3063380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75cc333a34f7788294e590abc79600965f6cf2d3f8561dbed33adc0362fd0c`  
		Last Modified: Wed, 13 Oct 2021 18:16:23 GMT  
		Size: 55.8 MB (55802879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d0466145763c731bdea690ba220239abbd35ca06ab4a5aa668c8e5b1510315`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:343086eb10fea1d0e294d959366776bd9cd3527c2b8f78ca2b41a25ce57f7c04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202133811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf5f72b35bd546cc8491264dba7674efb2a02f82fb9dea6db538ed870c4522b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 16:03:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:03:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:03:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:03:51 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:41:44 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:42:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:42:47 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:42:48 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:42:48 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:42:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:42:51 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:42:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:42:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:44:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:44:45 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:44:45 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:44:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:44:46 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:44:46 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba726e6e9acd11bec848488e1d9ba1dd28603662a05cb961c478edf2dfb5897b`  
		Last Modified: Tue, 12 Oct 2021 16:23:37 GMT  
		Size: 14.0 MB (13992252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfdcccd0ac8347312f70337b19af20dff7404116557f68a2ecddf40d033a66`  
		Last Modified: Tue, 12 Oct 2021 16:23:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d43d0920022abbdbd2439bdbfc251a541a3312219812894a15104cbc36da451`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c9895082195c18acb3a1950bccbfb998972a2a19b629d0e896b63ff2e9786c`  
		Last Modified: Wed, 13 Oct 2021 03:53:03 GMT  
		Size: 95.7 MB (95702557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fdcdc153d4a0f4d19f41c12cb4136e6879e01aae4b46e54ccd246aacf8509`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2705eeb2a9eaf702125ec2c318782eb4f43d41117ac7c7f2dab36275112d0b3`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb661f169d61250b0e2722b5df44b38e86dfe23c77a7d89e2871f7067e6b1e7`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 3.1 MB (3063242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143e4562d00275914a9d8cc6aad9335737e0bafde273ef01ce97c216fb8d73bd`  
		Last Modified: Wed, 13 Oct 2021 03:52:39 GMT  
		Size: 44.4 MB (44353070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4cf1b02b914b02976906375ae2c1c362060af22baccb8ed548f6a40b930399`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:a4c48b2c0bbb76d20734a3239c5ff4486fb06902d9161041f74716b4da26ab4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219642463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21372e7251d350b037972153cf0703df9289044566d5c57094d019c86f77787`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 18:52:55 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 18:53:00 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 18:53:05 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 18:59:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 18:59:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 18:59:55 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:46:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:46:53 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:46:59 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:47:04 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:47:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:47:21 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 14 Oct 2021 00:47:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 14 Oct 2021 00:47:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 00:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 00:52:57 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 00:53:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 00:53:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 00:53:25 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 00:53:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421cf7b60e6ecf3d6ad60b357e419014d8f6ad271c958a247f07c42e24664d11`  
		Last Modified: Tue, 12 Oct 2021 19:32:25 GMT  
		Size: 15.0 MB (14997040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06540a2f04ef35b100c723361f0086cb3542d114ee0eea90d820e05137d9c5dc`  
		Last Modified: Tue, 12 Oct 2021 19:32:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718e7a16edeab031c20f2c31cd9a6f1421c88037a4dfcf8b59604f89539cd11`  
		Last Modified: Thu, 14 Oct 2021 01:20:37 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a889dd8c5dd31d494ac35831e782d265b2bfe457db83677f7c047312896493`  
		Last Modified: Thu, 14 Oct 2021 01:21:41 GMT  
		Size: 101.3 MB (101327529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca7ef034d38ef39e783753bbb082ce26ec6fdd002cf9a68ce51058795ad8573`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232465c4db3849de029290c3113d2e54c170959078f1c6db79be04f25679d9`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ee5c28f159c990af395a85aca6dd92d3e5df1db87f1d1b22dd971db191ffa0`  
		Last Modified: Thu, 14 Oct 2021 01:20:33 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea081b840509c49626aada5a751b15f06425894b1909de76d192b435f459d`  
		Last Modified: Thu, 14 Oct 2021 01:20:40 GMT  
		Size: 57.0 MB (56997726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af764c7ef4e285b105b1dfdd393764172a828c880727596371b3d095e4fcd5`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:2d2e87d503c62c577e846a38406e5c4a17b470e0aff9daa3d535ad926ed37084
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202563722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a0171ae100a0cc3078e21c5b0bc20844d39c2bcebcf79ca3c96a0dc2c81552`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 04:18:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:18:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:18:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:18:07 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:35:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:36:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:36:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:36:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:36:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:36:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 09:36:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:38:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:38:07 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:38:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:38:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:38:07 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:38:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5683829b72e9a4d66e64d82641db943f6743e6c70a9a696d5ecee3d2bf6d2b5f`  
		Last Modified: Tue, 12 Oct 2021 04:31:02 GMT  
		Size: 14.7 MB (14697069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe5e8ef560af46263eb3ebe0e4907eeec84b5f7449bda56fd1cc07f5d84e234`  
		Last Modified: Tue, 12 Oct 2021 04:31:00 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b986a39650e8c61b28fb2e7aad4c6967ee7053443d5dd0f238431e9df00ed`  
		Last Modified: Tue, 12 Oct 2021 09:44:01 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e60616cc73d3b71b45dd0abf5d150c14c873b71026a5d817bb84fe76d32df5`  
		Last Modified: Tue, 12 Oct 2021 09:44:13 GMT  
		Size: 91.8 MB (91790121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a5fe3e5668c6414afc329a80c0981f446460312ec614052ea55a4b08d7e46f`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8ac8ca9b149047ed48dcb25ad3be07111b971715f73d0375a395b3a27af965`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960d15f81c4c390cd09bd901489ce0b96bbccda8a5f2bcd15f0243ae2df9d99`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25229088271a14206c72d9bf135c45e47af738e5da50cee70fd9d1821500b547`  
		Last Modified: Tue, 12 Oct 2021 09:44:04 GMT  
		Size: 56.4 MB (56439455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d605facdd969ae1f1091b22c319f219b199e11c31a4a879a23d7fe92d50d8307`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:cf4ec4d559c84d289809ddc6554057e6522d3720200a340c70ba098c12202c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:518ba4effd92c427ef19922743eea649ed001436d8a66fe0de469abb2de00949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149044368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48a04de41bf1795abeee36effc817551b3de5069209d3ec827816281c81211a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_MAJOR=2.7
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 13 Nov 2021 06:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 13 Nov 2021 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:47:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:47:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:47:56 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:28:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:29:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:29:07 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:29:08 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:29:08 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_VERSION=4.2.3
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Sat, 13 Nov 2021 14:29:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:29:13 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:31:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:31:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:31:22 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:31:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81c0605571c3961987ae1ce872ebef2b5bcb439010c194e90b47282556c32d`  
		Last Modified: Sat, 13 Nov 2021 06:58:25 GMT  
		Size: 14.0 MB (13994126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2814005984530d27bc89e1c810fb8cb01371038a28bc3d85a1e95b710d9e043e`  
		Last Modified: Sat, 13 Nov 2021 06:58:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171914095295d927972128e1f66156ce389cb697d40fc6d7ea68c919861015e`  
		Last Modified: Sat, 13 Nov 2021 14:36:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9802858485f172f49a49aa23ebc2ef97aa9a7dff598d4d6b18f27e107ae24436`  
		Last Modified: Sat, 13 Nov 2021 14:36:55 GMT  
		Size: 69.5 MB (69548252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5b29e3b352df46dbdcf96478507ab2ace06abee4b91e86cea6852a73067d98`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd79647c11e0ebdbaa7b41c71d969403768f7950e69f1b9eda5545fe42e86b3`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20504c29a1f01e91c83c2e1e82a90fb05c118bbf74d44fa621ec588a179bce4b`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 3.1 MB (3064272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d43b9df6162fdd2b107724ff288c851a49738e7e04fa16cd34fddde661b04`  
		Last Modified: Sat, 13 Nov 2021 14:36:48 GMT  
		Size: 56.0 MB (56029256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561c4b4d66001dcdc5ff09131812075d6a6d4f6430e175565724033921e826f1`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:0a2beba76e007d174f23a2648bb6286f22d459f02c4e52c079b233cc06019f18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:5df4cc2cc1a71f5966a962dabe733bb283f5dcf2d5d79c9a624ca4d234f974b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221663528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88e23cfd35a24f595790cf1434facb584b62ba6518a62473675f114c5bed8f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:11 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:46:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:46:36 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:46:36 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:46:36 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284a323be9f6611677ab116846d6c4dbf712313bcce34cf3e2c684501d18e10`  
		Last Modified: Wed, 10 Nov 2021 03:48:08 GMT  
		Size: 21.2 MB (21238255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebe82b2f5ac28b2b6826a4aec1e29a72892ccea15a741fc388f2c686094da69`  
		Last Modified: Wed, 10 Nov 2021 03:48:06 GMT  
		Size: 4.9 MB (4924623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:3cebf2567b163c5832fad36b21500a2c47df387f20c00f0103bb77581b7ba187
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

### `redmine:4.0` - linux; amd64

```console
$ docker pull redmine@sha256:d05e6d530735e8d5881f9327bc659a02f02ce7f3ea58110618f15c69d39e9ffd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205079351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b7e713d64f6b3d4959f4e70f1d18cba600919a28f04615191c094a5f47f7e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:23:19 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:23:20 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:23:20 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:23:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 20:23:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:25:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:25:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:25:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:25:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:25:54 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:25:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866c61464640233522ebdc402ab1639ef563ce15f4e766f0d2c9c46dbf47749`  
		Last Modified: Tue, 12 Oct 2021 20:29:14 GMT  
		Size: 81.2 MB (81200401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14796236954476acf9820e11bdeba8b19f45bff173cce221292a37501351dbfa`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f04093222ab3c15896fea65f4415539848dfd324ae9899f30a662a277b53939`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b703fd11a89eae2882c03999cd46f929263f1a53e9db14fca0d3a22402e65899`  
		Last Modified: Tue, 12 Oct 2021 20:28:55 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc91c4594f36a6f07f59f99aea2b24d308de0799bab28a2877ed2b560cbbef`  
		Last Modified: Tue, 12 Oct 2021 20:29:05 GMT  
		Size: 60.2 MB (60159580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474e32e03341c2aa37028e650008f2aef23216356cb3099c1fdd66d1190edfd9`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:76bde531fa51e9043ec26a480294be0bf2afa573b89eb6eee1c363d9b0061dae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194735396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a62e304aa3370634bf65d28936336cbe23efb8ac202b18443990b1dae175e34`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 07:20:59 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 07:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:25:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:25:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:13:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:23:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:23:43 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:23:44 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:23:45 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:23:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:23:47 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 03:23:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 03:23:53 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:30:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:30:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:30:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:30:56 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:30:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee56be0d198078cdceb927f259d279ea37548abbdefb95d8056e7e15d8137f0`  
		Last Modified: Tue, 12 Oct 2021 07:35:42 GMT  
		Size: 20.7 MB (20733372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e080526cffc142b881616db7396494f86cda539f9b9c65296f73498b8f70f81`  
		Last Modified: Tue, 12 Oct 2021 07:35:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c030517df14ac43613f1cd4bf516123c442ce7a9e6f545e593cc52a6b40fd301`  
		Last Modified: Wed, 13 Oct 2021 03:33:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d678b665817d824792999b8bfe1097e772d539be20d87a21b7856e05e68b96fa`  
		Last Modified: Wed, 13 Oct 2021 03:34:44 GMT  
		Size: 77.0 MB (76964464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268c5fac0a25fcda1e7b6e81b957c6ec41cd2a5e036ed031571f4d6c58f6b24`  
		Last Modified: Wed, 13 Oct 2021 03:34:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf21e0e9c72ebe28c5f11acc6887fd712ea95c2cd076725f01a2e89180c497`  
		Last Modified: Wed, 13 Oct 2021 03:34:06 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9804dc5e809a3c7310004b9c8e2d88e4a5a96fc1b4478080c2e4d4ce0585657b`  
		Last Modified: Wed, 13 Oct 2021 03:34:09 GMT  
		Size: 2.5 MB (2542539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d5a7b6ab1fa20d89537dbdd96653f63725bc98e85e648b81062fe647ca6c2`  
		Last Modified: Wed, 13 Oct 2021 03:34:29 GMT  
		Size: 59.3 MB (59268769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f02d814ee294160e2f9f09d190a6ed3a13b32c93990b2cb5ca48e819f88596`  
		Last Modified: Wed, 13 Oct 2021 03:34:07 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:a4c280bbf76f9bba2834f9064504ed314608d46e14f36ced5448faaa80a44bc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188068236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e8a6d08e93ea1d782be23860355520573e87862ab0ee514e619646b9cb223e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:29:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 03:33:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:33:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:33:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:33:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:41:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:49:21 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:49:22 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:49:22 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:49:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:49:25 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 06:49:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 06:49:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:55:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:55:07 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:55:08 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:55:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:55:08 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:55:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c9c99e0177bf2b2564708b982b9c36357cd8d40692351ae3fb607492c43c90`  
		Last Modified: Tue, 12 Oct 2021 03:42:55 GMT  
		Size: 20.6 MB (20643669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb852a3aed1bbfa0863f056cd080fad5debc62aefa369421cb364fde8137ebf`  
		Last Modified: Tue, 12 Oct 2021 03:42:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1086d0917a940899c5d3bad3fc3feea5fe65219a792b2acd69cd9ada062a7b`  
		Last Modified: Wed, 13 Oct 2021 06:57:14 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb023e9c4cb9847d03887a1e74509d1006934f33f168f7767fa3d0cfbb8993a`  
		Last Modified: Wed, 13 Oct 2021 06:59:10 GMT  
		Size: 73.3 MB (73263173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0734a96aee601c48b488de39bdd899a39839fbaefdc1985bc857df450c198d`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517f5edd505304a5cef2b06581a9ef09936a60ee7a42294579ea2c03b3d56ac`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcbad9cf302ea0ce760081905d9900133ec90ce11fd39b09fbdf9c488257498`  
		Last Modified: Wed, 13 Oct 2021 06:58:26 GMT  
		Size: 2.5 MB (2542549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd922d77362506a9ce9e94dd73d4abe3e913ecce129f542af606401d53107264`  
		Last Modified: Wed, 13 Oct 2021 06:58:51 GMT  
		Size: 59.0 MB (59002007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dd7573f2ae3e4eba3c72bbaed2d55ca28ac46b39bac2a652358df5ca161b6c`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:c744f7bdfc2b8fa61bb0d002f185732afcf33866e080fa88ae27ba8d03e11039
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.4 MB (200420198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cdd2517ddcf784d60fbe36c6aede4d86d0783059c6084084b411a20d686ab49`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:38:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 13 Oct 2021 17:38:59 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 13 Oct 2021 17:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 13 Oct 2021 17:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:40:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:40:47 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:10:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:13:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:13:35 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:13:36 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:13:37 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:13:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:13:39 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 18:13:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 18:13:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:15:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:15:49 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:15:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:15:52 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:15:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e089afb774d84c5dff2c325f7155a5e3b024317dfc7a765993bee56d59b284b2`  
		Last Modified: Wed, 13 Oct 2021 17:51:29 GMT  
		Size: 21.1 MB (21095215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8bc5a0e22361e7e8e0ddabf3d6dbd6c21343f2a70438b440df94c72265632`  
		Last Modified: Wed, 13 Oct 2021 17:51:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b617a973d96061be3c87fdd4e1f8ce3d07e80d9bec144dd8101856eeb18b73f`  
		Last Modified: Wed, 13 Oct 2021 18:17:10 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071415292e5b7e0c2b687a88c0f9793010b755c3e4c665db989723911dc4fddb`  
		Last Modified: Wed, 13 Oct 2021 18:17:50 GMT  
		Size: 79.8 MB (79758464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e13094544110d6f242c41c786d2185aff41581b1b839fa9dea1246b37dc1446`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27282c349cc3168fddb7e34c18eb14ab4e3b6429c33b3d58224961205e9c21a0`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb138819a2da803e898f97433cb248a3bfc694b70b19387bb8596d69a787c5`  
		Last Modified: Wed, 13 Oct 2021 18:17:36 GMT  
		Size: 2.5 MB (2543982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd4f06db06834ac4490d7d578febd92d5db79c118a6c771f395d9f0fa90e3f`  
		Last Modified: Wed, 13 Oct 2021 18:17:43 GMT  
		Size: 59.8 MB (59848248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62029c47a85bca5fa7aea14b0185b755ca7004ba5697f583d0aab6a24ef23bb`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:2ebb4f7f48b83283d9e1673ad235bdc6eedb95310e613ee75d3edd5699087f53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210334021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98cf580c7851d9200dd869f67b83e6ba27c272f4713570715af798c995cccee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 16:13:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 16:16:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:16:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:16:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:16:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:44:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:48:45 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:48:46 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:48:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:48:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:48:49 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 03:48:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 03:48:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:51:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:51:50 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:51:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:51:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:51:50 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:51:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67095d3fd063e93bf9a3c675db4f6e3400c4be3693ed130eef2e6e6b069cf364`  
		Last Modified: Tue, 12 Oct 2021 16:24:59 GMT  
		Size: 20.9 MB (20910155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea2fc65b147afe00cf84051e64271787774a8fe6fcefafb4a556fbe54e8ff3`  
		Last Modified: Tue, 12 Oct 2021 16:24:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b42b1ec6770d2595d0abd4da13a43bdd8abe29533047c17d2edc5dd650405`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0958703ae525d9d151d6a97fa54ccc49192bcfa143a50a448afe030a7f658d`  
		Last Modified: Wed, 13 Oct 2021 03:54:34 GMT  
		Size: 82.6 MB (82599870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5950d0dadfd613d687edf87b02ac7952395ed8c78618b85435c70cf4fbb70c71`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa87c54c48a338759cba269e0b627047e4394c5feb7479173bf9dd25bec25e1`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3ac64d4724594ce6921879a687c5a0546cbdf8b0b9d50e64467f4033ad3bb3`  
		Last Modified: Wed, 13 Oct 2021 03:54:06 GMT  
		Size: 2.5 MB (2542551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af552c5db1efb93e18dfeba25d6837af16dcaa5890143d026c473a23f6d687b7`  
		Last Modified: Wed, 13 Oct 2021 03:54:20 GMT  
		Size: 59.3 MB (59258756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1545ca19158d289b01567199840caa306023ff9a5d455d4e0aab3872f6aa7f`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:6aac498c44f600b672d9897703c3c41b214924e3fc233e7860fd8e545b136e77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216469674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4da6045a34b42bbefc251f10d5f010773a1e6f3bcfc1555ea6958d409fbead`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 19:17:28 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 19:17:32 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 19:17:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 19:25:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 19:25:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 19:26:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 19:26:22 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:54:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 01:07:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 01:08:11 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 01:08:23 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 01:08:27 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 01:08:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 01:08:47 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 14 Oct 2021 01:08:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 14 Oct 2021 01:09:18 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 01:19:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 01:19:19 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 01:19:23 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 01:19:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 01:19:47 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 01:19:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03211df41d3c61789be71d89ebad2ce881638fb2a84c27562d7e3ff81f181458`  
		Last Modified: Tue, 12 Oct 2021 19:33:41 GMT  
		Size: 22.0 MB (21984973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c774747b6862c16e290d0508df2db39d1a24d4061e198d3567c877d14ca4bf8`  
		Last Modified: Tue, 12 Oct 2021 19:33:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d344e083cdb889978f1a8f40a20c569e9d02d096352f103edc1381edd38d39a`  
		Last Modified: Thu, 14 Oct 2021 01:22:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac438230a35738c21d025cb57c8c2c12a0694fc9dcafd9d3f1f1cc5d52cac12`  
		Last Modified: Thu, 14 Oct 2021 01:22:55 GMT  
		Size: 87.9 MB (87902632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96411f53dc60a5c0667e24e7007ead33f7a43d92b6c882aa193e719f58ed663`  
		Last Modified: Thu, 14 Oct 2021 01:22:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2634382c5d445a0bba90dc55ead78291350aad0aa956fe9f87bbaa4f73cdfed`  
		Last Modified: Thu, 14 Oct 2021 01:22:37 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17f74adf31cae17cfb0a926e812563f2f59c5c7778cc5f8d84e26e09015218`  
		Last Modified: Thu, 14 Oct 2021 01:22:37 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce9fa655873ae250f6f495e0d5433626b0bba0c00566e89e82fcadc94703ea4`  
		Last Modified: Thu, 14 Oct 2021 01:22:45 GMT  
		Size: 60.8 MB (60782595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df59993b68006e819fad6adcd54c3e76dc6dc32f43f6b365d3a69aa8e22b1b35`  
		Last Modified: Thu, 14 Oct 2021 01:22:36 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:8139940ee123294a1f3c9d391f88e4315d31fd439375dc258513aa7ddc1570f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200275204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6dc1405d64f3fbd0d0a205989b62e8dc0be10c6f7d4b53f3b3e32208fcb76e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:38:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:41:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:41:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:41:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:41:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:41:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:41:17 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 09:41:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 09:41:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:43:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:43:33 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:43:33 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:43:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:43:33 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:43:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c171029d31b91789b83992e2df8d28e67db9b64aee10772ef9305c5fa5d911`  
		Last Modified: Tue, 12 Oct 2021 09:44:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0353fa71ce129db2fdca57a1c5e738cd3889b519fceb96f005a67980d01dc260`  
		Last Modified: Tue, 12 Oct 2021 09:44:56 GMT  
		Size: 78.9 MB (78942069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b228dd835e5f8743a168736313e3d9db3607d5ceede6d35ead9175c7efd972e`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8ab59b6b034b6c4f909fb6333a2d962568fe81001bc663f99e7180615705e`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf85425cb344073d010664c8b0c3cb2bc16f419cba15f2863c966e4bea8c88be`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 2.5 MB (2542537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7688eafc5b2a7028f0f3777a04b615bd8e406826e3ffb2830466f8d233e533`  
		Last Modified: Tue, 12 Oct 2021 09:44:51 GMT  
		Size: 60.6 MB (60597020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab25a5872446bdc8315bb901e91b80b748fd30a7722eda73cc43e0856d5256`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:fa8ba213e2dfef7bfb98c3b2ca6af9917a9c0b9b15be67bb8c20499ac3d04aed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:01887efbc27065bcc544e6ba80201b994e89e27280c7b25de2c280d6f1b33024
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153558063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4abb35ae9e45f8c5510f9bfe3efa808d3e893645c29b1b6aa08bae910bf2aa9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 13 Nov 2021 06:51:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 13 Nov 2021 06:54:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:54:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:54:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:54:46 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:31:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:34:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Sat, 13 Nov 2021 14:34:29 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:34:29 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:34:29 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:34:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:34:30 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 13 Nov 2021 14:34:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 13 Nov 2021 14:34:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:34:34 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:36:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:36:07 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:36:07 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:36:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:36:07 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:36:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd76747f3be3e4f4af1119b668fd5a9fa53725f84b429575cfb26c0d5f842a`  
		Last Modified: Sat, 13 Nov 2021 06:59:00 GMT  
		Size: 19.5 MB (19500293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bbfb1229cd3c27d4dd990a0daf591e427afbc679b854303415a9e9a01ff10b`  
		Last Modified: Sat, 13 Nov 2021 06:58:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267c2d73515a2e4fbaac349e5a31212348b7d72b21f80611dac1923c5c68666`  
		Last Modified: Sat, 13 Nov 2021 14:37:15 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ea963f3d5877eea0043f8a2b75f17680ff5a4d362c1a4fce8c8a67c347239`  
		Last Modified: Sat, 13 Nov 2021 14:37:49 GMT  
		Size: 66.2 MB (66199469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05071f335bb9135d55d21c80aaa3523ae388d93f1a98136404e7c91fa99fb524`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a43db45233bb37a8a7df21efee11df06d119f141dd51e3c8672893a9bb6a654`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb71bc10f9decb3a165b48fa2dae4aa79929b41c812f261a1ff1fee173510e8`  
		Last Modified: Sat, 13 Nov 2021 14:37:38 GMT  
		Size: 2.5 MB (2543762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d38dd936d4bdfa095bb3270305cfe38c97043649fdf48ba25879b221ebbb40`  
		Last Modified: Sat, 13 Nov 2021 14:37:43 GMT  
		Size: 58.9 MB (58906080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac236fd681e485d4f3495d7195078b72db1997782784f2aca237835c80c236`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:8f5dc49e7e8b0e12174df5fa85995971245c971765697ba9c8d5dfedbf1181c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ab67f320b1123ca1304a82c786eae4039d20fd4c88b83296db005396040c20c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231443403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f098d154d4397a6cf6ab16cf24d877414f42e3f0e229c0f85ebbc51d47fc41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:23:19 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:23:20 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:23:20 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:23:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 20:23:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:25:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:25:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:25:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:25:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:25:54 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:25:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:47:10 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:47:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:47:29 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:47:29 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:47:29 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866c61464640233522ebdc402ab1639ef563ce15f4e766f0d2c9c46dbf47749`  
		Last Modified: Tue, 12 Oct 2021 20:29:14 GMT  
		Size: 81.2 MB (81200401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14796236954476acf9820e11bdeba8b19f45bff173cce221292a37501351dbfa`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f04093222ab3c15896fea65f4415539848dfd324ae9899f30a662a277b53939`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b703fd11a89eae2882c03999cd46f929263f1a53e9db14fca0d3a22402e65899`  
		Last Modified: Tue, 12 Oct 2021 20:28:55 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc91c4594f36a6f07f59f99aea2b24d308de0799bab28a2877ed2b560cbbef`  
		Last Modified: Tue, 12 Oct 2021 20:29:05 GMT  
		Size: 60.2 MB (60159580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474e32e03341c2aa37028e650008f2aef23216356cb3099c1fdd66d1190edfd9`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d8b5222950710a3689bed3c7d25c043a60ee6308b734dd7e9e3fb1cd20aecf`  
		Last Modified: Wed, 10 Nov 2021 03:48:45 GMT  
		Size: 21.4 MB (21439436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0429cf4f74ed45039bbed5c5f537f08b624eb8bd977152cd098f2b290c2c5dd0`  
		Last Modified: Wed, 10 Nov 2021 03:48:43 GMT  
		Size: 4.9 MB (4924616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9`

```console
$ docker pull redmine@sha256:3cebf2567b163c5832fad36b21500a2c47df387f20c00f0103bb77581b7ba187
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

### `redmine:4.0.9` - linux; amd64

```console
$ docker pull redmine@sha256:d05e6d530735e8d5881f9327bc659a02f02ce7f3ea58110618f15c69d39e9ffd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205079351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6b7e713d64f6b3d4959f4e70f1d18cba600919a28f04615191c094a5f47f7e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:23:19 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:23:20 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:23:20 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:23:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 20:23:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:25:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:25:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:25:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:25:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:25:54 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:25:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866c61464640233522ebdc402ab1639ef563ce15f4e766f0d2c9c46dbf47749`  
		Last Modified: Tue, 12 Oct 2021 20:29:14 GMT  
		Size: 81.2 MB (81200401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14796236954476acf9820e11bdeba8b19f45bff173cce221292a37501351dbfa`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f04093222ab3c15896fea65f4415539848dfd324ae9899f30a662a277b53939`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b703fd11a89eae2882c03999cd46f929263f1a53e9db14fca0d3a22402e65899`  
		Last Modified: Tue, 12 Oct 2021 20:28:55 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc91c4594f36a6f07f59f99aea2b24d308de0799bab28a2877ed2b560cbbef`  
		Last Modified: Tue, 12 Oct 2021 20:29:05 GMT  
		Size: 60.2 MB (60159580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474e32e03341c2aa37028e650008f2aef23216356cb3099c1fdd66d1190edfd9`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v5

```console
$ docker pull redmine@sha256:76bde531fa51e9043ec26a480294be0bf2afa573b89eb6eee1c363d9b0061dae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194735396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a62e304aa3370634bf65d28936336cbe23efb8ac202b18443990b1dae175e34`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 07:20:59 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 07:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:25:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:25:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:13:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:23:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:23:43 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:23:44 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:23:45 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:23:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:23:47 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 03:23:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 03:23:53 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:30:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:30:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:30:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:30:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:30:56 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:30:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee56be0d198078cdceb927f259d279ea37548abbdefb95d8056e7e15d8137f0`  
		Last Modified: Tue, 12 Oct 2021 07:35:42 GMT  
		Size: 20.7 MB (20733372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e080526cffc142b881616db7396494f86cda539f9b9c65296f73498b8f70f81`  
		Last Modified: Tue, 12 Oct 2021 07:35:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c030517df14ac43613f1cd4bf516123c442ce7a9e6f545e593cc52a6b40fd301`  
		Last Modified: Wed, 13 Oct 2021 03:33:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d678b665817d824792999b8bfe1097e772d539be20d87a21b7856e05e68b96fa`  
		Last Modified: Wed, 13 Oct 2021 03:34:44 GMT  
		Size: 77.0 MB (76964464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268c5fac0a25fcda1e7b6e81b957c6ec41cd2a5e036ed031571f4d6c58f6b24`  
		Last Modified: Wed, 13 Oct 2021 03:34:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf21e0e9c72ebe28c5f11acc6887fd712ea95c2cd076725f01a2e89180c497`  
		Last Modified: Wed, 13 Oct 2021 03:34:06 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9804dc5e809a3c7310004b9c8e2d88e4a5a96fc1b4478080c2e4d4ce0585657b`  
		Last Modified: Wed, 13 Oct 2021 03:34:09 GMT  
		Size: 2.5 MB (2542539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d5a7b6ab1fa20d89537dbdd96653f63725bc98e85e648b81062fe647ca6c2`  
		Last Modified: Wed, 13 Oct 2021 03:34:29 GMT  
		Size: 59.3 MB (59268769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f02d814ee294160e2f9f09d190a6ed3a13b32c93990b2cb5ca48e819f88596`  
		Last Modified: Wed, 13 Oct 2021 03:34:07 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v7

```console
$ docker pull redmine@sha256:a4c280bbf76f9bba2834f9064504ed314608d46e14f36ced5448faaa80a44bc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188068236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e8a6d08e93ea1d782be23860355520573e87862ab0ee514e619646b9cb223e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:29:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 03:33:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:33:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:33:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:33:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:41:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:49:21 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:49:22 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:49:22 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:49:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:49:25 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 06:49:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 06:49:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:55:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:55:07 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:55:08 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:55:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:55:08 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:55:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c9c99e0177bf2b2564708b982b9c36357cd8d40692351ae3fb607492c43c90`  
		Last Modified: Tue, 12 Oct 2021 03:42:55 GMT  
		Size: 20.6 MB (20643669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb852a3aed1bbfa0863f056cd080fad5debc62aefa369421cb364fde8137ebf`  
		Last Modified: Tue, 12 Oct 2021 03:42:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1086d0917a940899c5d3bad3fc3feea5fe65219a792b2acd69cd9ada062a7b`  
		Last Modified: Wed, 13 Oct 2021 06:57:14 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb023e9c4cb9847d03887a1e74509d1006934f33f168f7767fa3d0cfbb8993a`  
		Last Modified: Wed, 13 Oct 2021 06:59:10 GMT  
		Size: 73.3 MB (73263173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0734a96aee601c48b488de39bdd899a39839fbaefdc1985bc857df450c198d`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517f5edd505304a5cef2b06581a9ef09936a60ee7a42294579ea2c03b3d56ac`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcbad9cf302ea0ce760081905d9900133ec90ce11fd39b09fbdf9c488257498`  
		Last Modified: Wed, 13 Oct 2021 06:58:26 GMT  
		Size: 2.5 MB (2542549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd922d77362506a9ce9e94dd73d4abe3e913ecce129f542af606401d53107264`  
		Last Modified: Wed, 13 Oct 2021 06:58:51 GMT  
		Size: 59.0 MB (59002007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dd7573f2ae3e4eba3c72bbaed2d55ca28ac46b39bac2a652358df5ca161b6c`  
		Last Modified: Wed, 13 Oct 2021 06:58:22 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:c744f7bdfc2b8fa61bb0d002f185732afcf33866e080fa88ae27ba8d03e11039
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.4 MB (200420198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cdd2517ddcf784d60fbe36c6aede4d86d0783059c6084084b411a20d686ab49`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:38:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 13 Oct 2021 17:38:59 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 13 Oct 2021 17:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 13 Oct 2021 17:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:40:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:40:47 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:10:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:13:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:13:35 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:13:36 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:13:37 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:13:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:13:39 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 18:13:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 18:13:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:15:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:15:49 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:15:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:15:52 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:15:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e089afb774d84c5dff2c325f7155a5e3b024317dfc7a765993bee56d59b284b2`  
		Last Modified: Wed, 13 Oct 2021 17:51:29 GMT  
		Size: 21.1 MB (21095215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8bc5a0e22361e7e8e0ddabf3d6dbd6c21343f2a70438b440df94c72265632`  
		Last Modified: Wed, 13 Oct 2021 17:51:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b617a973d96061be3c87fdd4e1f8ce3d07e80d9bec144dd8101856eeb18b73f`  
		Last Modified: Wed, 13 Oct 2021 18:17:10 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071415292e5b7e0c2b687a88c0f9793010b755c3e4c665db989723911dc4fddb`  
		Last Modified: Wed, 13 Oct 2021 18:17:50 GMT  
		Size: 79.8 MB (79758464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e13094544110d6f242c41c786d2185aff41581b1b839fa9dea1246b37dc1446`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27282c349cc3168fddb7e34c18eb14ab4e3b6429c33b3d58224961205e9c21a0`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb138819a2da803e898f97433cb248a3bfc694b70b19387bb8596d69a787c5`  
		Last Modified: Wed, 13 Oct 2021 18:17:36 GMT  
		Size: 2.5 MB (2543982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfd4f06db06834ac4490d7d578febd92d5db79c118a6c771f395d9f0fa90e3f`  
		Last Modified: Wed, 13 Oct 2021 18:17:43 GMT  
		Size: 59.8 MB (59848248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62029c47a85bca5fa7aea14b0185b755ca7004ba5697f583d0aab6a24ef23bb`  
		Last Modified: Wed, 13 Oct 2021 18:17:35 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; 386

```console
$ docker pull redmine@sha256:2ebb4f7f48b83283d9e1673ad235bdc6eedb95310e613ee75d3edd5699087f53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210334021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f98cf580c7851d9200dd869f67b83e6ba27c272f4713570715af798c995cccee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 16:13:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 16:16:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:16:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:16:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:16:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:44:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:48:45 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:48:46 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:48:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:48:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:48:49 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 13 Oct 2021 03:48:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 13 Oct 2021 03:48:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:51:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:51:50 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:51:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:51:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:51:50 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:51:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67095d3fd063e93bf9a3c675db4f6e3400c4be3693ed130eef2e6e6b069cf364`  
		Last Modified: Tue, 12 Oct 2021 16:24:59 GMT  
		Size: 20.9 MB (20910155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea2fc65b147afe00cf84051e64271787774a8fe6fcefafb4a556fbe54e8ff3`  
		Last Modified: Tue, 12 Oct 2021 16:24:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b42b1ec6770d2595d0abd4da13a43bdd8abe29533047c17d2edc5dd650405`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0958703ae525d9d151d6a97fa54ccc49192bcfa143a50a448afe030a7f658d`  
		Last Modified: Wed, 13 Oct 2021 03:54:34 GMT  
		Size: 82.6 MB (82599870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5950d0dadfd613d687edf87b02ac7952395ed8c78618b85435c70cf4fbb70c71`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa87c54c48a338759cba269e0b627047e4394c5feb7479173bf9dd25bec25e1`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3ac64d4724594ce6921879a687c5a0546cbdf8b0b9d50e64467f4033ad3bb3`  
		Last Modified: Wed, 13 Oct 2021 03:54:06 GMT  
		Size: 2.5 MB (2542551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af552c5db1efb93e18dfeba25d6837af16dcaa5890143d026c473a23f6d687b7`  
		Last Modified: Wed, 13 Oct 2021 03:54:20 GMT  
		Size: 59.3 MB (59258756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1545ca19158d289b01567199840caa306023ff9a5d455d4e0aab3872f6aa7f`  
		Last Modified: Wed, 13 Oct 2021 03:54:05 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; ppc64le

```console
$ docker pull redmine@sha256:6aac498c44f600b672d9897703c3c41b214924e3fc233e7860fd8e545b136e77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216469674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f4da6045a34b42bbefc251f10d5f010773a1e6f3bcfc1555ea6958d409fbead`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 19:17:28 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 19:17:32 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 19:17:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 19:25:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 19:25:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 19:26:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 19:26:22 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:54:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 01:07:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 01:08:11 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 01:08:23 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 01:08:27 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 01:08:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 01:08:47 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 14 Oct 2021 01:08:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 14 Oct 2021 01:09:18 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 01:19:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 01:19:19 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 01:19:23 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 01:19:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 01:19:47 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 01:19:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03211df41d3c61789be71d89ebad2ce881638fb2a84c27562d7e3ff81f181458`  
		Last Modified: Tue, 12 Oct 2021 19:33:41 GMT  
		Size: 22.0 MB (21984973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c774747b6862c16e290d0508df2db39d1a24d4061e198d3567c877d14ca4bf8`  
		Last Modified: Tue, 12 Oct 2021 19:33:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d344e083cdb889978f1a8f40a20c569e9d02d096352f103edc1381edd38d39a`  
		Last Modified: Thu, 14 Oct 2021 01:22:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac438230a35738c21d025cb57c8c2c12a0694fc9dcafd9d3f1f1cc5d52cac12`  
		Last Modified: Thu, 14 Oct 2021 01:22:55 GMT  
		Size: 87.9 MB (87902632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96411f53dc60a5c0667e24e7007ead33f7a43d92b6c882aa193e719f58ed663`  
		Last Modified: Thu, 14 Oct 2021 01:22:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2634382c5d445a0bba90dc55ead78291350aad0aa956fe9f87bbaa4f73cdfed`  
		Last Modified: Thu, 14 Oct 2021 01:22:37 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e17f74adf31cae17cfb0a926e812563f2f59c5c7778cc5f8d84e26e09015218`  
		Last Modified: Thu, 14 Oct 2021 01:22:37 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce9fa655873ae250f6f495e0d5433626b0bba0c00566e89e82fcadc94703ea4`  
		Last Modified: Thu, 14 Oct 2021 01:22:45 GMT  
		Size: 60.8 MB (60782595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df59993b68006e819fad6adcd54c3e76dc6dc32f43f6b365d3a69aa8e22b1b35`  
		Last Modified: Thu, 14 Oct 2021 01:22:36 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; s390x

```console
$ docker pull redmine@sha256:8139940ee123294a1f3c9d391f88e4315d31fd439375dc258513aa7ddc1570f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200275204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6dc1405d64f3fbd0d0a205989b62e8dc0be10c6f7d4b53f3b3e32208fcb76e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:38:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:41:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:41:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:41:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:41:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:41:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:41:17 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 09:41:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 09:41:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:43:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:43:33 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:43:33 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:43:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:43:33 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:43:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c171029d31b91789b83992e2df8d28e67db9b64aee10772ef9305c5fa5d911`  
		Last Modified: Tue, 12 Oct 2021 09:44:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0353fa71ce129db2fdca57a1c5e738cd3889b519fceb96f005a67980d01dc260`  
		Last Modified: Tue, 12 Oct 2021 09:44:56 GMT  
		Size: 78.9 MB (78942069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b228dd835e5f8743a168736313e3d9db3607d5ceede6d35ead9175c7efd972e`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8ab59b6b034b6c4f909fb6333a2d962568fe81001bc663f99e7180615705e`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf85425cb344073d010664c8b0c3cb2bc16f419cba15f2863c966e4bea8c88be`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 2.5 MB (2542537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7688eafc5b2a7028f0f3777a04b615bd8e406826e3ffb2830466f8d233e533`  
		Last Modified: Tue, 12 Oct 2021 09:44:51 GMT  
		Size: 60.6 MB (60597020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab25a5872446bdc8315bb901e91b80b748fd30a7722eda73cc43e0856d5256`  
		Last Modified: Tue, 12 Oct 2021 09:44:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-alpine`

```console
$ docker pull redmine@sha256:fa8ba213e2dfef7bfb98c3b2ca6af9917a9c0b9b15be67bb8c20499ac3d04aed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0.9-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:01887efbc27065bcc544e6ba80201b994e89e27280c7b25de2c280d6f1b33024
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153558063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4abb35ae9e45f8c5510f9bfe3efa808d3e893645c29b1b6aa08bae910bf2aa9a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 13 Nov 2021 06:51:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 13 Nov 2021 06:54:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:54:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:54:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:54:46 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:31:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:34:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Sat, 13 Nov 2021 14:34:29 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:34:29 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:34:29 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:34:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:34:30 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 13 Nov 2021 14:34:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 13 Nov 2021 14:34:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:34:34 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:36:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:36:07 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:36:07 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:36:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:36:07 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:36:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd76747f3be3e4f4af1119b668fd5a9fa53725f84b429575cfb26c0d5f842a`  
		Last Modified: Sat, 13 Nov 2021 06:59:00 GMT  
		Size: 19.5 MB (19500293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bbfb1229cd3c27d4dd990a0daf591e427afbc679b854303415a9e9a01ff10b`  
		Last Modified: Sat, 13 Nov 2021 06:58:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267c2d73515a2e4fbaac349e5a31212348b7d72b21f80611dac1923c5c68666`  
		Last Modified: Sat, 13 Nov 2021 14:37:15 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ea963f3d5877eea0043f8a2b75f17680ff5a4d362c1a4fce8c8a67c347239`  
		Last Modified: Sat, 13 Nov 2021 14:37:49 GMT  
		Size: 66.2 MB (66199469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05071f335bb9135d55d21c80aaa3523ae388d93f1a98136404e7c91fa99fb524`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a43db45233bb37a8a7df21efee11df06d119f141dd51e3c8672893a9bb6a654`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb71bc10f9decb3a165b48fa2dae4aa79929b41c812f261a1ff1fee173510e8`  
		Last Modified: Sat, 13 Nov 2021 14:37:38 GMT  
		Size: 2.5 MB (2543762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d38dd936d4bdfa095bb3270305cfe38c97043649fdf48ba25879b221ebbb40`  
		Last Modified: Sat, 13 Nov 2021 14:37:43 GMT  
		Size: 58.9 MB (58906080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac236fd681e485d4f3495d7195078b72db1997782784f2aca237835c80c236`  
		Last Modified: Sat, 13 Nov 2021 14:37:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-passenger`

```console
$ docker pull redmine@sha256:8f5dc49e7e8b0e12174df5fa85995971245c971765697ba9c8d5dfedbf1181c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0.9-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ab67f320b1123ca1304a82c786eae4039d20fd4c88b83296db005396040c20c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231443403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f098d154d4397a6cf6ab16cf24d877414f42e3f0e229c0f85ebbc51d47fc41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:23:19 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:23:20 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:23:20 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:23:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 12 Oct 2021 20:23:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 12 Oct 2021 20:23:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:25:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:25:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:25:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:25:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:25:54 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:25:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:47:10 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:47:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:47:29 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:47:29 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:47:29 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5866c61464640233522ebdc402ab1639ef563ce15f4e766f0d2c9c46dbf47749`  
		Last Modified: Tue, 12 Oct 2021 20:29:14 GMT  
		Size: 81.2 MB (81200401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14796236954476acf9820e11bdeba8b19f45bff173cce221292a37501351dbfa`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f04093222ab3c15896fea65f4415539848dfd324ae9899f30a662a277b53939`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b703fd11a89eae2882c03999cd46f929263f1a53e9db14fca0d3a22402e65899`  
		Last Modified: Tue, 12 Oct 2021 20:28:55 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc91c4594f36a6f07f59f99aea2b24d308de0799bab28a2877ed2b560cbbef`  
		Last Modified: Tue, 12 Oct 2021 20:29:05 GMT  
		Size: 60.2 MB (60159580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474e32e03341c2aa37028e650008f2aef23216356cb3099c1fdd66d1190edfd9`  
		Last Modified: Tue, 12 Oct 2021 20:28:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d8b5222950710a3689bed3c7d25c043a60ee6308b734dd7e9e3fb1cd20aecf`  
		Last Modified: Wed, 10 Nov 2021 03:48:45 GMT  
		Size: 21.4 MB (21439436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0429cf4f74ed45039bbed5c5f537f08b624eb8bd977152cd098f2b290c2c5dd0`  
		Last Modified: Wed, 10 Nov 2021 03:48:43 GMT  
		Size: 4.9 MB (4924616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:e8a8defc97f2413cef87c8f633abd01251c26c847dc06d84bd23b7149a4da025
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

### `redmine:4.1` - linux; amd64

```console
$ docker pull redmine@sha256:403c93eb007bd16cd277e19fc1459f180c7483fa4940fd5044a30acef53a8f01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206668627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0da7de9c6f21204eac2ef99bfd1d097808059ad4f8daeb89898eb83deffb97c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:20:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:20:57 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:20:57 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:20:57 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:20:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 20:21:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:22:14 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:22:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:22:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:22:15 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:22:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8617ac0503291a7bc25ab3e9ecadad7f36606e38768ec7dae57decbca32bc1ea`  
		Last Modified: Tue, 12 Oct 2021 20:28:29 GMT  
		Size: 94.1 MB (94088241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a76df102ee332891a671c026db6214352f68c057230bbdae139ea2227fe745`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f353dd18278378e4d8216c008d56bc846a5a701d5a7730f60698a69cc659c8b`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888176d4f29df43b84ccec41ac92479f77bee993d76d41344d933ff075acec4`  
		Last Modified: Tue, 12 Oct 2021 20:28:11 GMT  
		Size: 2.7 MB (2749692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edea4661341065395429e13204ddb02ce8e2608365b08a4b649071683624d43`  
		Last Modified: Tue, 12 Oct 2021 20:28:17 GMT  
		Size: 48.7 MB (48653871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811deb43f4603834d18cf1fe5b28601cc92f816a4dbc984fe9858936d4f44a3`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:fd9a6ca83808905c079ff29662f81bb35330a8be3abbc339c2507c971852ea3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210669047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fb4a19021b4eeca711ee785701e0df1d7d03e3e0871a30ad557c336a06e2ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 07:20:59 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 07:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:25:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:25:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:13:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:15:19 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:15:21 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:15:22 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:15:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:15:28 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 03:15:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 03:15:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:22:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:22:12 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:22:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:22:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:22:15 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:22:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee56be0d198078cdceb927f259d279ea37548abbdefb95d8056e7e15d8137f0`  
		Last Modified: Tue, 12 Oct 2021 07:35:42 GMT  
		Size: 20.7 MB (20733372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e080526cffc142b881616db7396494f86cda539f9b9c65296f73498b8f70f81`  
		Last Modified: Tue, 12 Oct 2021 07:35:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c030517df14ac43613f1cd4bf516123c442ce7a9e6f545e593cc52a6b40fd301`  
		Last Modified: Wed, 13 Oct 2021 03:33:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3897ec5e588606be8744330bf1c4d14efe3cb454ad1a7a28841648516085a681`  
		Last Modified: Wed, 13 Oct 2021 03:33:53 GMT  
		Size: 89.6 MB (89575164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14263ed54825c7939921f07b976fdeb8d1030283ae7629fb3cad48bcad63ef8b`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42977913dd4d9c9fc4f9bbe0ec0c1cf86191be9b169e4625fd52638bd2d6990`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc078b0610e878e98fe32bd23535bba23460228cdb6d1c9342420cc1056fb1`  
		Last Modified: Wed, 13 Oct 2021 03:33:11 GMT  
		Size: 2.7 MB (2749695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435301d2e3e6d0eb02ef7f3dfef10b39d778154c1dbca332274b48b117a3a9e`  
		Last Modified: Wed, 13 Oct 2021 03:33:31 GMT  
		Size: 62.4 MB (62384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b775033255d5a1a789c784df094106b9b2489c0a159ff5d254d4e9c670b6084f`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:380b2a1bd20ab586d27fccfa9e704b5711d53271b5ae1ea0b553d0dff129aa5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203851889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a22805d3ff7605300793419e632f413f2e1715dc0ccaf9dc46bb5cff553b7b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:29:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 03:33:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:33:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:33:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:33:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:41:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:42:35 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:42:36 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:42:36 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:42:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:42:38 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 06:42:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 06:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:48:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:48:02 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:48:03 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:48:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:48:04 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:48:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c9c99e0177bf2b2564708b982b9c36357cd8d40692351ae3fb607492c43c90`  
		Last Modified: Tue, 12 Oct 2021 03:42:55 GMT  
		Size: 20.6 MB (20643669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb852a3aed1bbfa0863f056cd080fad5debc62aefa369421cb364fde8137ebf`  
		Last Modified: Tue, 12 Oct 2021 03:42:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1086d0917a940899c5d3bad3fc3feea5fe65219a792b2acd69cd9ada062a7b`  
		Last Modified: Wed, 13 Oct 2021 06:57:14 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd9f426d70a745f2ddce33d8ac46330d64fcbed546853bad59d21f3534ca535`  
		Last Modified: Wed, 13 Oct 2021 06:58:10 GMT  
		Size: 85.6 MB (85590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3942a6e72dd3e213cd5889c3c17e56b4b1ff4c59a01feeab202d71714b219`  
		Last Modified: Wed, 13 Oct 2021 06:57:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706f62754dfee343ce1dbe89f0c2c61bc69c76aaabdfeec1b1dbb316c723f046`  
		Last Modified: Wed, 13 Oct 2021 06:57:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afaba210f3f7cccc352f3a2bfb91fcfe93bbc146f42e038f0bf03d42a628754`  
		Last Modified: Wed, 13 Oct 2021 06:57:16 GMT  
		Size: 2.7 MB (2749696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e3e7f892fb877ae9658d4cf0c4c042302426527d05083af6384970cbeb8c12`  
		Last Modified: Wed, 13 Oct 2021 06:57:41 GMT  
		Size: 62.3 MB (62251280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a5677793c6ff5ebcc5d032b27aaef548b1be3fd53835a226127d26743d3d34`  
		Last Modified: Wed, 13 Oct 2021 06:57:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:fd06ad39105508320a9cd34cae0aedf31c2bd2bd35f5b3a2f469f06fb0c05c4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217092058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943edc29cd283d9208b6a49f9da243d361cc6a84cea5c9dfd1e1e1139760b49d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:38:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 13 Oct 2021 17:38:59 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 13 Oct 2021 17:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 13 Oct 2021 17:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:40:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:40:47 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:10:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:10:42 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:10:43 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:10:44 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:10:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:10:46 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 18:10:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 18:10:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:13:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:13:02 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:13:03 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:13:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:13:05 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:13:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e089afb774d84c5dff2c325f7155a5e3b024317dfc7a765993bee56d59b284b2`  
		Last Modified: Wed, 13 Oct 2021 17:51:29 GMT  
		Size: 21.1 MB (21095215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8bc5a0e22361e7e8e0ddabf3d6dbd6c21343f2a70438b440df94c72265632`  
		Last Modified: Wed, 13 Oct 2021 17:51:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b617a973d96061be3c87fdd4e1f8ce3d07e80d9bec144dd8101856eeb18b73f`  
		Last Modified: Wed, 13 Oct 2021 18:17:10 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e88c6504a5141bbb7273d56ca4e3f9a55730f5791e4ac1a3b550b7495fd32d`  
		Last Modified: Wed, 13 Oct 2021 18:17:24 GMT  
		Size: 92.6 MB (92615053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b54d1c515bdbdf4d68fc006173eef4697b152e6c813a461a1cf5abd1ffbbb`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecee8043f87e3e01143ca4d85bb3c3c3460be99ed04de6a596df1d5a1df7346`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f149084a4be44f9e72d3685c0511f21ff853157bf38f6d4f4f2f7ccb05d9c06`  
		Last Modified: Wed, 13 Oct 2021 18:17:09 GMT  
		Size: 2.7 MB (2749624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29388f4c9cd02c9816fb0e9234674601e0756cfacf8b1aeec276fce263774a9`  
		Last Modified: Wed, 13 Oct 2021 18:17:16 GMT  
		Size: 63.5 MB (63457875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4119a9a565721870dc37ac880f6df259d99983d59c23e9012886172d1890e01b`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:f7567e0e07de03585db57a1e8cdd7b890988ef514213172695ba399de82b2b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213020802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59627d0765e640768b0f0485669face5eb9a10330782273b6bc395ecbaf49a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 16:13:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 16:16:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:16:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:16:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:16:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:44:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:45:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:45:58 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:45:58 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:45:58 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:46:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:46:01 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 03:46:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 03:46:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:47:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:47:38 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:47:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:47:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:47:40 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:47:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67095d3fd063e93bf9a3c675db4f6e3400c4be3693ed130eef2e6e6b069cf364`  
		Last Modified: Tue, 12 Oct 2021 16:24:59 GMT  
		Size: 20.9 MB (20910155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea2fc65b147afe00cf84051e64271787774a8fe6fcefafb4a556fbe54e8ff3`  
		Last Modified: Tue, 12 Oct 2021 16:24:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b42b1ec6770d2595d0abd4da13a43bdd8abe29533047c17d2edc5dd650405`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91496d867c1bb245f5d002c23b2eecabdb2014aa2cb71cd493a9e077cb4391`  
		Last Modified: Wed, 13 Oct 2021 03:53:53 GMT  
		Size: 95.7 MB (95702712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9126fedc0229f00ab5e28d08dc42314e1aa4aa11a9f0ab626215c349a344633`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed73609e6e04848f78656ca2dc96a0e4fc4ab040204baf8ad6a790bf6b784d9`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a1b5e50a9ef35e90705203009bd0f42dd9058ebff857cb472b4bebb04c541`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 2.7 MB (2749691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43629c12985f8bb524ddbb6270f6b679083ac0890096e2b51ccb7c2528fdc599`  
		Last Modified: Wed, 13 Oct 2021 03:53:37 GMT  
		Size: 48.6 MB (48635554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d930778c61e685c5f1c40e603a80b2b3ad4afddf3ee65861f97750ec818b6fdc`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:5044f07ac6e60e5b6a94218b4fa90ac3d73d57d97a26f2e2cf04d94e1a315f71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234111493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2794e91b1bd4c9b3e213162f8b7cb1f15f81466089a83cfe972eccaae93c389`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 19:17:28 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 19:17:32 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 19:17:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 19:25:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 19:25:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 19:26:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 19:26:22 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:54:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:57:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:57:57 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:58:08 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:58:13 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:58:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:58:35 GMT
ENV REDMINE_VERSION=4.1.5
# Thu, 14 Oct 2021 00:58:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Thu, 14 Oct 2021 00:59:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 01:04:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 01:04:25 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 01:04:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 01:04:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 01:04:36 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 01:04:45 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03211df41d3c61789be71d89ebad2ce881638fb2a84c27562d7e3ff81f181458`  
		Last Modified: Tue, 12 Oct 2021 19:33:41 GMT  
		Size: 22.0 MB (21984973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c774747b6862c16e290d0508df2db39d1a24d4061e198d3567c877d14ca4bf8`  
		Last Modified: Tue, 12 Oct 2021 19:33:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d344e083cdb889978f1a8f40a20c569e9d02d096352f103edc1381edd38d39a`  
		Last Modified: Thu, 14 Oct 2021 01:22:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055091d203c828eda50c0fc58b4fc2380bb289903300ac48506d41b11e3e64f6`  
		Last Modified: Thu, 14 Oct 2021 01:22:24 GMT  
		Size: 101.3 MB (101326908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aa33ed3b974244546104fc2f17c16cfc59c3961420d73a00dcdd428d919dbd`  
		Last Modified: Thu, 14 Oct 2021 01:22:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584682ab54558b6bba089db5b421b6d785c617bf43197cb9e72c61fc0c1cc4a8`  
		Last Modified: Thu, 14 Oct 2021 01:22:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f458104410b51d3994141d75dce44360cfa46fcc01e9f6d5cd2bea7491862f7`  
		Last Modified: Thu, 14 Oct 2021 01:22:02 GMT  
		Size: 2.7 MB (2749690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0ff33ddbb28614d7a7634c41197a24124d710178ee5f90ae4375482059c7d9`  
		Last Modified: Thu, 14 Oct 2021 01:22:10 GMT  
		Size: 64.8 MB (64792996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc93cfdeb63ee31180bf5ef1dae43d601a4102973a3654b4999e7c17912a573d`  
		Last Modified: Thu, 14 Oct 2021 01:22:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:5a28369651e18f9f1ce4f5196d816c9f738425c373d7bd715a5cbd4dc6b82316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216911533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48173507aadcad0fbe3a5b41c5d20279d8f57bc0678495af57e3af66533818a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:38:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:38:45 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:38:45 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:38:45 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:38:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:38:46 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 09:38:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 09:38:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:40:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:40:32 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:40:32 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:40:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:40:32 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:40:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c171029d31b91789b83992e2df8d28e67db9b64aee10772ef9305c5fa5d911`  
		Last Modified: Tue, 12 Oct 2021 09:44:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1c209b3a3e0cbd64f1ae7b80c081f013e6b193c2f42cda5eb7b9ad626a87a0`  
		Last Modified: Tue, 12 Oct 2021 09:44:38 GMT  
		Size: 91.8 MB (91790331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8c7cb055eaab704bfb028353639ec47986c91928cf2fd1a8c4cab80b27c28`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5ae1c9cdf8e055ca7a459b5956e54c8cf0a9e45a64e1175ae159d3b91b70bd`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27474e63020bc20f6ebca29d511f9bc83f72c68555614f2ed401483c7a0faf13`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 2.7 MB (2749688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9ad44a4e87c764d5f92243c086a8636cd58979093416ddbb98c59feafd488c`  
		Last Modified: Tue, 12 Oct 2021 09:44:30 GMT  
		Size: 64.2 MB (64177934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7759dd1acaed2d5bd99f0da4deb3b1a51cac6e8af980dc41bca73a02aed08c`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:6dbd35c35e023b696f652aa87bf1de330ef19513a1b85a00928f30244c701767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:fae3d2c173aad1c4ccf2ae887f62847716af5f908fa917fbac07b10913b45913
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160030996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4714a18668c5842cac48a8a5bf13f3af01f3662dadbd9b44c49730c89b727d24`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 13 Nov 2021 06:51:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 13 Nov 2021 06:54:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:54:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:54:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:54:46 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:31:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:31:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:31:48 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:31:49 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:31:49 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:31:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:31:50 GMT
ENV REDMINE_VERSION=4.1.5
# Sat, 13 Nov 2021 14:31:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Sat, 13 Nov 2021 14:31:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:31:54 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:34:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:34:01 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:34:01 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:34:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:34:02 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:34:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd76747f3be3e4f4af1119b668fd5a9fa53725f84b429575cfb26c0d5f842a`  
		Last Modified: Sat, 13 Nov 2021 06:59:00 GMT  
		Size: 19.5 MB (19500293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bbfb1229cd3c27d4dd990a0daf591e427afbc679b854303415a9e9a01ff10b`  
		Last Modified: Sat, 13 Nov 2021 06:58:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267c2d73515a2e4fbaac349e5a31212348b7d72b21f80611dac1923c5c68666`  
		Last Modified: Sat, 13 Nov 2021 14:37:15 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e62a0f0fc43b5aab817648e0aea8e8dcd39e0f5e7ee6ce76236ac5f49653e2`  
		Last Modified: Sat, 13 Nov 2021 14:37:25 GMT  
		Size: 69.5 MB (69547670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ce34581c9e5eb65bc5ed69717166b196e1a17a8607e3721ae1b07c1cb90c8`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a2fb4d61b7d1eb854991664d217dae48916bd3cf240c27f4fa2534973b40a5`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6afa58a2a007900b48af7fe611027ca52ed3c1034ea34e75d6db8dddb5b18d1`  
		Last Modified: Sat, 13 Nov 2021 14:37:14 GMT  
		Size: 2.8 MB (2750433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a6c05fbcb5a65730f500ffa36488a9d0667133c3c4e784f88e4c8c966f946c`  
		Last Modified: Sat, 13 Nov 2021 14:37:19 GMT  
		Size: 61.8 MB (61824139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03693e88b691e6215bdd51b25ee8b9e56f1967a1ee89d59e4ecc12f354cbcb28`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:d5a0a1c46c5bec1cf4b1e4fea37df3e3afe64ad7565b9654a0b8e63253f1664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b3b58664ca0f89c6644786cf4723d0e788734e3703b0fdd046165f5be908c80c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233029805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552964d89f045555c3d775895653aff55ca34c34ee435419b869aaf1f374b966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:20:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:20:57 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:20:57 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:20:57 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:20:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 20:21:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:22:14 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:22:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:22:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:22:15 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:22:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:43 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:47:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:47:03 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:47:03 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:47:03 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8617ac0503291a7bc25ab3e9ecadad7f36606e38768ec7dae57decbca32bc1ea`  
		Last Modified: Tue, 12 Oct 2021 20:28:29 GMT  
		Size: 94.1 MB (94088241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a76df102ee332891a671c026db6214352f68c057230bbdae139ea2227fe745`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f353dd18278378e4d8216c008d56bc846a5a701d5a7730f60698a69cc659c8b`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888176d4f29df43b84ccec41ac92479f77bee993d76d41344d933ff075acec4`  
		Last Modified: Tue, 12 Oct 2021 20:28:11 GMT  
		Size: 2.7 MB (2749692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edea4661341065395429e13204ddb02ce8e2608365b08a4b649071683624d43`  
		Last Modified: Tue, 12 Oct 2021 20:28:17 GMT  
		Size: 48.7 MB (48653871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811deb43f4603834d18cf1fe5b28601cc92f816a4dbc984fe9858936d4f44a3`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90d10b267c49cba83436d1bad2aa20653bde9c3681fbe2277d43a2ef691e5d`  
		Last Modified: Wed, 10 Nov 2021 03:48:30 GMT  
		Size: 21.4 MB (21436536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff182f4aaf60af77237f70493b14e2c05a22437378c9d91850db63454081120`  
		Last Modified: Wed, 10 Nov 2021 03:48:28 GMT  
		Size: 4.9 MB (4924642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.5`

```console
$ docker pull redmine@sha256:e8a8defc97f2413cef87c8f633abd01251c26c847dc06d84bd23b7149a4da025
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

### `redmine:4.1.5` - linux; amd64

```console
$ docker pull redmine@sha256:403c93eb007bd16cd277e19fc1459f180c7483fa4940fd5044a30acef53a8f01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206668627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0da7de9c6f21204eac2ef99bfd1d097808059ad4f8daeb89898eb83deffb97c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:20:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:20:57 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:20:57 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:20:57 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:20:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 20:21:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:22:14 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:22:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:22:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:22:15 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:22:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8617ac0503291a7bc25ab3e9ecadad7f36606e38768ec7dae57decbca32bc1ea`  
		Last Modified: Tue, 12 Oct 2021 20:28:29 GMT  
		Size: 94.1 MB (94088241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a76df102ee332891a671c026db6214352f68c057230bbdae139ea2227fe745`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f353dd18278378e4d8216c008d56bc846a5a701d5a7730f60698a69cc659c8b`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888176d4f29df43b84ccec41ac92479f77bee993d76d41344d933ff075acec4`  
		Last Modified: Tue, 12 Oct 2021 20:28:11 GMT  
		Size: 2.7 MB (2749692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edea4661341065395429e13204ddb02ce8e2608365b08a4b649071683624d43`  
		Last Modified: Tue, 12 Oct 2021 20:28:17 GMT  
		Size: 48.7 MB (48653871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811deb43f4603834d18cf1fe5b28601cc92f816a4dbc984fe9858936d4f44a3`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; arm variant v5

```console
$ docker pull redmine@sha256:fd9a6ca83808905c079ff29662f81bb35330a8be3abbc339c2507c971852ea3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210669047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fb4a19021b4eeca711ee785701e0df1d7d03e3e0871a30ad557c336a06e2ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 07:20:58 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 07:20:59 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 07:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:25:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:25:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:25:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:13:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:15:19 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:15:21 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:15:22 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:15:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:15:28 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 03:15:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 03:15:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:22:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:22:12 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:22:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:22:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:22:15 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:22:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee56be0d198078cdceb927f259d279ea37548abbdefb95d8056e7e15d8137f0`  
		Last Modified: Tue, 12 Oct 2021 07:35:42 GMT  
		Size: 20.7 MB (20733372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e080526cffc142b881616db7396494f86cda539f9b9c65296f73498b8f70f81`  
		Last Modified: Tue, 12 Oct 2021 07:35:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c030517df14ac43613f1cd4bf516123c442ce7a9e6f545e593cc52a6b40fd301`  
		Last Modified: Wed, 13 Oct 2021 03:33:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3897ec5e588606be8744330bf1c4d14efe3cb454ad1a7a28841648516085a681`  
		Last Modified: Wed, 13 Oct 2021 03:33:53 GMT  
		Size: 89.6 MB (89575164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14263ed54825c7939921f07b976fdeb8d1030283ae7629fb3cad48bcad63ef8b`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42977913dd4d9c9fc4f9bbe0ec0c1cf86191be9b169e4625fd52638bd2d6990`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fc078b0610e878e98fe32bd23535bba23460228cdb6d1c9342420cc1056fb1`  
		Last Modified: Wed, 13 Oct 2021 03:33:11 GMT  
		Size: 2.7 MB (2749695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435301d2e3e6d0eb02ef7f3dfef10b39d778154c1dbca332274b48b117a3a9e`  
		Last Modified: Wed, 13 Oct 2021 03:33:31 GMT  
		Size: 62.4 MB (62384562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b775033255d5a1a789c784df094106b9b2489c0a159ff5d254d4e9c670b6084f`  
		Last Modified: Wed, 13 Oct 2021 03:33:09 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; arm variant v7

```console
$ docker pull redmine@sha256:380b2a1bd20ab586d27fccfa9e704b5711d53271b5ae1ea0b553d0dff129aa5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203851889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a22805d3ff7605300793419e632f413f2e1715dc0ccaf9dc46bb5cff553b7b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:29:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 03:29:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 03:33:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:33:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:33:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:33:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:33:33 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:41:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:42:35 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:42:36 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:42:36 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:42:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:42:38 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 06:42:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 06:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:48:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:48:02 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:48:03 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:48:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:48:04 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:48:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c9c99e0177bf2b2564708b982b9c36357cd8d40692351ae3fb607492c43c90`  
		Last Modified: Tue, 12 Oct 2021 03:42:55 GMT  
		Size: 20.6 MB (20643669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb852a3aed1bbfa0863f056cd080fad5debc62aefa369421cb364fde8137ebf`  
		Last Modified: Tue, 12 Oct 2021 03:42:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1086d0917a940899c5d3bad3fc3feea5fe65219a792b2acd69cd9ada062a7b`  
		Last Modified: Wed, 13 Oct 2021 06:57:14 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd9f426d70a745f2ddce33d8ac46330d64fcbed546853bad59d21f3534ca535`  
		Last Modified: Wed, 13 Oct 2021 06:58:10 GMT  
		Size: 85.6 MB (85590404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3942a6e72dd3e213cd5889c3c17e56b4b1ff4c59a01feeab202d71714b219`  
		Last Modified: Wed, 13 Oct 2021 06:57:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706f62754dfee343ce1dbe89f0c2c61bc69c76aaabdfeec1b1dbb316c723f046`  
		Last Modified: Wed, 13 Oct 2021 06:57:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afaba210f3f7cccc352f3a2bfb91fcfe93bbc146f42e038f0bf03d42a628754`  
		Last Modified: Wed, 13 Oct 2021 06:57:16 GMT  
		Size: 2.7 MB (2749696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e3e7f892fb877ae9658d4cf0c4c042302426527d05083af6384970cbeb8c12`  
		Last Modified: Wed, 13 Oct 2021 06:57:41 GMT  
		Size: 62.3 MB (62251280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a5677793c6ff5ebcc5d032b27aaef548b1be3fd53835a226127d26743d3d34`  
		Last Modified: Wed, 13 Oct 2021 06:57:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:fd06ad39105508320a9cd34cae0aedf31c2bd2bd35f5b3a2f469f06fb0c05c4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217092058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943edc29cd283d9208b6a49f9da243d361cc6a84cea5c9dfd1e1e1139760b49d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:38:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 13 Oct 2021 17:38:59 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 13 Oct 2021 17:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 13 Oct 2021 17:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:40:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:40:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:40:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:40:47 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:10:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:10:42 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:10:43 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:10:44 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:10:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:10:46 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 18:10:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 18:10:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:13:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:13:02 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:13:03 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:13:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:13:05 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:13:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e089afb774d84c5dff2c325f7155a5e3b024317dfc7a765993bee56d59b284b2`  
		Last Modified: Wed, 13 Oct 2021 17:51:29 GMT  
		Size: 21.1 MB (21095215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8bc5a0e22361e7e8e0ddabf3d6dbd6c21343f2a70438b440df94c72265632`  
		Last Modified: Wed, 13 Oct 2021 17:51:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b617a973d96061be3c87fdd4e1f8ce3d07e80d9bec144dd8101856eeb18b73f`  
		Last Modified: Wed, 13 Oct 2021 18:17:10 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e88c6504a5141bbb7273d56ca4e3f9a55730f5791e4ac1a3b550b7495fd32d`  
		Last Modified: Wed, 13 Oct 2021 18:17:24 GMT  
		Size: 92.6 MB (92615053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b54d1c515bdbdf4d68fc006173eef4697b152e6c813a461a1cf5abd1ffbbb`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecee8043f87e3e01143ca4d85bb3c3c3460be99ed04de6a596df1d5a1df7346`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f149084a4be44f9e72d3685c0511f21ff853157bf38f6d4f4f2f7ccb05d9c06`  
		Last Modified: Wed, 13 Oct 2021 18:17:09 GMT  
		Size: 2.7 MB (2749624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29388f4c9cd02c9816fb0e9234674601e0756cfacf8b1aeec276fce263774a9`  
		Last Modified: Wed, 13 Oct 2021 18:17:16 GMT  
		Size: 63.5 MB (63457875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4119a9a565721870dc37ac880f6df259d99983d59c23e9012886172d1890e01b`  
		Last Modified: Wed, 13 Oct 2021 18:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; 386

```console
$ docker pull redmine@sha256:f7567e0e07de03585db57a1e8cdd7b890988ef514213172695ba399de82b2b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213020802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f59627d0765e640768b0f0485669face5eb9a10330782273b6bc395ecbaf49a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 16:13:57 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 16:13:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 16:16:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:16:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:16:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:16:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:16:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:44:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:45:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:45:58 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:45:58 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:45:58 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:46:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:46:01 GMT
ENV REDMINE_VERSION=4.1.5
# Wed, 13 Oct 2021 03:46:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Wed, 13 Oct 2021 03:46:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:47:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:47:38 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:47:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:47:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:47:40 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:47:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67095d3fd063e93bf9a3c675db4f6e3400c4be3693ed130eef2e6e6b069cf364`  
		Last Modified: Tue, 12 Oct 2021 16:24:59 GMT  
		Size: 20.9 MB (20910155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ea2fc65b147afe00cf84051e64271787774a8fe6fcefafb4a556fbe54e8ff3`  
		Last Modified: Tue, 12 Oct 2021 16:24:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b42b1ec6770d2595d0abd4da13a43bdd8abe29533047c17d2edc5dd650405`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91496d867c1bb245f5d002c23b2eecabdb2014aa2cb71cd493a9e077cb4391`  
		Last Modified: Wed, 13 Oct 2021 03:53:53 GMT  
		Size: 95.7 MB (95702712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9126fedc0229f00ab5e28d08dc42314e1aa4aa11a9f0ab626215c349a344633`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed73609e6e04848f78656ca2dc96a0e4fc4ab040204baf8ad6a790bf6b784d9`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a1b5e50a9ef35e90705203009bd0f42dd9058ebff857cb472b4bebb04c541`  
		Last Modified: Wed, 13 Oct 2021 03:53:28 GMT  
		Size: 2.7 MB (2749691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43629c12985f8bb524ddbb6270f6b679083ac0890096e2b51ccb7c2528fdc599`  
		Last Modified: Wed, 13 Oct 2021 03:53:37 GMT  
		Size: 48.6 MB (48635554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d930778c61e685c5f1c40e603a80b2b3ad4afddf3ee65861f97750ec818b6fdc`  
		Last Modified: Wed, 13 Oct 2021 03:53:26 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; ppc64le

```console
$ docker pull redmine@sha256:5044f07ac6e60e5b6a94218b4fa90ac3d73d57d97a26f2e2cf04d94e1a315f71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234111493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2794e91b1bd4c9b3e213162f8b7cb1f15f81466089a83cfe972eccaae93c389`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 19:17:28 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 19:17:32 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 19:17:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 19:25:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 19:25:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 19:26:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 19:26:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 19:26:22 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:54:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:57:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:57:57 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:58:08 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:58:13 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:58:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:58:35 GMT
ENV REDMINE_VERSION=4.1.5
# Thu, 14 Oct 2021 00:58:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Thu, 14 Oct 2021 00:59:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 01:04:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 01:04:25 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 01:04:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 01:04:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 01:04:36 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 01:04:45 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03211df41d3c61789be71d89ebad2ce881638fb2a84c27562d7e3ff81f181458`  
		Last Modified: Tue, 12 Oct 2021 19:33:41 GMT  
		Size: 22.0 MB (21984973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c774747b6862c16e290d0508df2db39d1a24d4061e198d3567c877d14ca4bf8`  
		Last Modified: Tue, 12 Oct 2021 19:33:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d344e083cdb889978f1a8f40a20c569e9d02d096352f103edc1381edd38d39a`  
		Last Modified: Thu, 14 Oct 2021 01:22:07 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055091d203c828eda50c0fc58b4fc2380bb289903300ac48506d41b11e3e64f6`  
		Last Modified: Thu, 14 Oct 2021 01:22:24 GMT  
		Size: 101.3 MB (101326908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86aa33ed3b974244546104fc2f17c16cfc59c3961420d73a00dcdd428d919dbd`  
		Last Modified: Thu, 14 Oct 2021 01:22:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584682ab54558b6bba089db5b421b6d785c617bf43197cb9e72c61fc0c1cc4a8`  
		Last Modified: Thu, 14 Oct 2021 01:22:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f458104410b51d3994141d75dce44360cfa46fcc01e9f6d5cd2bea7491862f7`  
		Last Modified: Thu, 14 Oct 2021 01:22:02 GMT  
		Size: 2.7 MB (2749690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0ff33ddbb28614d7a7634c41197a24124d710178ee5f90ae4375482059c7d9`  
		Last Modified: Thu, 14 Oct 2021 01:22:10 GMT  
		Size: 64.8 MB (64792996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc93cfdeb63ee31180bf5ef1dae43d601a4102973a3654b4999e7c17912a573d`  
		Last Modified: Thu, 14 Oct 2021 01:22:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.5` - linux; s390x

```console
$ docker pull redmine@sha256:5a28369651e18f9f1ce4f5196d816c9f738425c373d7bd715a5cbd4dc6b82316
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216911533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48173507aadcad0fbe3a5b41c5d20279d8f57bc0678495af57e3af66533818a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:26:01 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 04:26:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 04:27:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:27:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:27:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:27:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:27:33 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:38:20 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:38:45 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:38:45 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:38:45 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:38:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:38:46 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 09:38:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 09:38:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:40:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:40:32 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:40:32 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:40:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:40:32 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:40:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58406908df2376127547311dc0ea98d9ef92a8573d1e0cb811fefa665bb3a84`  
		Last Modified: Tue, 12 Oct 2021 04:31:30 GMT  
		Size: 21.6 MB (21619749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4ab84de8ab158c29c0c84a1b4726fd7c89ab7ff6fb27c139956d200f492b2`  
		Last Modified: Tue, 12 Oct 2021 04:31:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c171029d31b91789b83992e2df8d28e67db9b64aee10772ef9305c5fa5d911`  
		Last Modified: Tue, 12 Oct 2021 09:44:26 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1c209b3a3e0cbd64f1ae7b80c081f013e6b193c2f42cda5eb7b9ad626a87a0`  
		Last Modified: Tue, 12 Oct 2021 09:44:38 GMT  
		Size: 91.8 MB (91790331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8c7cb055eaab704bfb028353639ec47986c91928cf2fd1a8c4cab80b27c28`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5ae1c9cdf8e055ca7a459b5956e54c8cf0a9e45a64e1175ae159d3b91b70bd`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27474e63020bc20f6ebca29d511f9bc83f72c68555614f2ed401483c7a0faf13`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 2.7 MB (2749688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9ad44a4e87c764d5f92243c086a8636cd58979093416ddbb98c59feafd488c`  
		Last Modified: Tue, 12 Oct 2021 09:44:30 GMT  
		Size: 64.2 MB (64177934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7759dd1acaed2d5bd99f0da4deb3b1a51cac6e8af980dc41bca73a02aed08c`  
		Last Modified: Tue, 12 Oct 2021 09:44:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.5-alpine`

```console
$ docker pull redmine@sha256:6dbd35c35e023b696f652aa87bf1de330ef19513a1b85a00928f30244c701767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.5-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:fae3d2c173aad1c4ccf2ae887f62847716af5f908fa917fbac07b10913b45913
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160030996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4714a18668c5842cac48a8a5bf13f3af01f3662dadbd9b44c49730c89b727d24`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 13 Nov 2021 06:51:30 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 13 Nov 2021 06:51:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 13 Nov 2021 06:54:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:54:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:54:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:54:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:54:46 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:31:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:31:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:31:48 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:31:49 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:31:49 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:31:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:31:50 GMT
ENV REDMINE_VERSION=4.1.5
# Sat, 13 Nov 2021 14:31:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Sat, 13 Nov 2021 14:31:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:31:54 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:34:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:34:01 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:34:01 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:34:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:34:02 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:34:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd76747f3be3e4f4af1119b668fd5a9fa53725f84b429575cfb26c0d5f842a`  
		Last Modified: Sat, 13 Nov 2021 06:59:00 GMT  
		Size: 19.5 MB (19500293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bbfb1229cd3c27d4dd990a0daf591e427afbc679b854303415a9e9a01ff10b`  
		Last Modified: Sat, 13 Nov 2021 06:58:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267c2d73515a2e4fbaac349e5a31212348b7d72b21f80611dac1923c5c68666`  
		Last Modified: Sat, 13 Nov 2021 14:37:15 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e62a0f0fc43b5aab817648e0aea8e8dcd39e0f5e7ee6ce76236ac5f49653e2`  
		Last Modified: Sat, 13 Nov 2021 14:37:25 GMT  
		Size: 69.5 MB (69547670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ce34581c9e5eb65bc5ed69717166b196e1a17a8607e3721ae1b07c1cb90c8`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a2fb4d61b7d1eb854991664d217dae48916bd3cf240c27f4fa2534973b40a5`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6afa58a2a007900b48af7fe611027ca52ed3c1034ea34e75d6db8dddb5b18d1`  
		Last Modified: Sat, 13 Nov 2021 14:37:14 GMT  
		Size: 2.8 MB (2750433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a6c05fbcb5a65730f500ffa36488a9d0667133c3c4e784f88e4c8c966f946c`  
		Last Modified: Sat, 13 Nov 2021 14:37:19 GMT  
		Size: 61.8 MB (61824139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03693e88b691e6215bdd51b25ee8b9e56f1967a1ee89d59e4ecc12f354cbcb28`  
		Last Modified: Sat, 13 Nov 2021 14:37:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.5-passenger`

```console
$ docker pull redmine@sha256:d5a0a1c46c5bec1cf4b1e4fea37df3e3afe64ad7565b9654a0b8e63253f1664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.5-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b3b58664ca0f89c6644786cf4723d0e788734e3703b0fdd046165f5be908c80c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233029805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:552964d89f045555c3d775895653aff55ca34c34ee435419b869aaf1f374b966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 12 Oct 2021 15:34:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 12 Oct 2021 15:37:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:37:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:37:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:37:06 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:20:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:20:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:20:57 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:20:57 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:20:57 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:20:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_VERSION=4.1.5
# Tue, 12 Oct 2021 20:20:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=624dfeab7db5cda35a03d791b5fa83a836717ca280856c51cd089ed638f8678e
# Tue, 12 Oct 2021 20:21:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:22:14 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:22:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:22:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:22:15 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:22:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:43 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:47:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:47:03 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:47:03 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:47:03 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc3e5ccddf2ccfcc978381549c751e1167cdf41ce60580404b33cb6fdd7aa5`  
		Last Modified: Tue, 12 Oct 2021 15:41:15 GMT  
		Size: 21.5 MB (21467885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b99a224b661061fbbe799d6efb95f01221754e6a73aec4d536865d1e304d63`  
		Last Modified: Tue, 12 Oct 2021 15:41:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b92be01811211d262d0872aabc77c74589ad10e263a5d091b7a77fc657edd4`  
		Last Modified: Tue, 12 Oct 2021 20:28:12 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8617ac0503291a7bc25ab3e9ecadad7f36606e38768ec7dae57decbca32bc1ea`  
		Last Modified: Tue, 12 Oct 2021 20:28:29 GMT  
		Size: 94.1 MB (94088241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a76df102ee332891a671c026db6214352f68c057230bbdae139ea2227fe745`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f353dd18278378e4d8216c008d56bc846a5a701d5a7730f60698a69cc659c8b`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888176d4f29df43b84ccec41ac92479f77bee993d76d41344d933ff075acec4`  
		Last Modified: Tue, 12 Oct 2021 20:28:11 GMT  
		Size: 2.7 MB (2749692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edea4661341065395429e13204ddb02ce8e2608365b08a4b649071683624d43`  
		Last Modified: Tue, 12 Oct 2021 20:28:17 GMT  
		Size: 48.7 MB (48653871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811deb43f4603834d18cf1fe5b28601cc92f816a4dbc984fe9858936d4f44a3`  
		Last Modified: Tue, 12 Oct 2021 20:28:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c90d10b267c49cba83436d1bad2aa20653bde9c3681fbe2277d43a2ef691e5d`  
		Last Modified: Wed, 10 Nov 2021 03:48:30 GMT  
		Size: 21.4 MB (21436536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff182f4aaf60af77237f70493b14e2c05a22437378c9d91850db63454081120`  
		Last Modified: Wed, 10 Nov 2021 03:48:28 GMT  
		Size: 4.9 MB (4924642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2`

```console
$ docker pull redmine@sha256:75c11d669206fefdb4e833f087be5a76327fe402ebda35ac41880656cf9c2128
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

### `redmine:4.2` - linux; amd64

```console
$ docker pull redmine@sha256:23da6bbd8146ba5ebc6c565af6a4941d0a836fb5f2b3cf8281d954a84047c675
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195500650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777ff92e6fdbdb00a6ebcf1c2df29c52c4cbb171e418bcee49451b9df8ddf3b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:08f124ad97cbf3d78e62b390897fbd0a6e47f4901f4ce4f632d68de47d1236c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196991904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750dc7fdc53efaea0a675c5102c8cc3d6c8e5fb47e2bb056eae33416edf86f72`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 07:03:18 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 07:07:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:07:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:07:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:07:39 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:06:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:06:17 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:06:19 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:06:20 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:06:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:06:24 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:06:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:06:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:13:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:13:17 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:13:19 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:13:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:13:22 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854afe8d48105a800902d829046a9890cab76441d450aa59877c28405734daed`  
		Last Modified: Tue, 12 Oct 2021 07:33:59 GMT  
		Size: 13.9 MB (13871429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97d908af060f6e00c4e7a607087a50b553e21e08c6a8c70274a3d81ea0b3ef`  
		Last Modified: Tue, 12 Oct 2021 07:33:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a08bb1308b5863e00403e1a34c4cb2a9aafa57091f2d1faa4936463e4f8de79`  
		Last Modified: Wed, 13 Oct 2021 03:32:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b177e5e016cce70192ebf1277d5a21559c74cf5aa60e6bff5dfb31a9d5767e8`  
		Last Modified: Wed, 13 Oct 2021 03:32:45 GMT  
		Size: 89.6 MB (89577077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa429c867c2a22535e2c33e168d8de14f69c6f13124dc7494d06630528d03c43`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168fe406bb1360b18d49546d4af05cccf7fb548d99e4f4663d83dab19f23f4be`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2ee921f4dfd9c1a73cfe3b44b39e67f1af385494dd03e3fe1cbdc9c31aaf1`  
		Last Modified: Wed, 13 Oct 2021 03:32:04 GMT  
		Size: 3.1 MB (3063249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892b495be3664dd078f8510b6b3222fec0b0eeceaaa8fcc540d7ced595ecf23`  
		Last Modified: Wed, 13 Oct 2021 03:32:21 GMT  
		Size: 55.3 MB (55253893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea12a2e245bbbc4585eb36f1a1709b9035c2beaac9e1be72d14f2bf9c84118e`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:900b0cad4acc6dc28f8f9e3279e4a10121c4d247bd540f66d7ff40fcdf914200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190138732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88b04a543401c43e354aa169b439ad085b11a2b6acbde3b9a6a36f4307bec08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 03:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:10:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:10:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:10:57 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:34:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:35:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:35:44 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:35:45 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:35:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:35:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:35:48 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 06:35:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 06:35:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:41:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:41:11 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:41:12 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:41:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ab36f90d94f50bb2f0b4be72799049691d9d0f05aadbe4e5cba89a3989efd1`  
		Last Modified: Tue, 12 Oct 2021 03:41:56 GMT  
		Size: 13.8 MB (13767235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a22941e2b0ce8584f2fa791a8370a30bd3a202fa73a1dd64d00a85bf075916a`  
		Last Modified: Tue, 12 Oct 2021 03:41:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6828dc1bb7b47f9d60169ee81885096702049306577ce953096d5057c12e91af`  
		Last Modified: Wed, 13 Oct 2021 06:55:56 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e9962d77928a7fea0f4dd24c838a24f72da3eba59ed75e59a3557633655398`  
		Last Modified: Wed, 13 Oct 2021 06:56:52 GMT  
		Size: 85.6 MB (85590281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894593e78f4567729a26e4302a660a56ee7289a18398fb9ec5b526be2466b739`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f705a0b143059f649ff99fd7d343002386794bfe675456f393697b71d9dbc5`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14825a50627a0f65eec1cc695fb3896ea4d8a22a09fc112bc902fcbbdd53be02`  
		Last Modified: Wed, 13 Oct 2021 06:56:03 GMT  
		Size: 3.1 MB (3063246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461661b0c3351479c43855bab9a39d5482ee87a52376bc2898c48b83ce9ada1`  
		Last Modified: Wed, 13 Oct 2021 06:56:20 GMT  
		Size: 55.1 MB (55101134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b2c0757c967dd445d6615d9fa9fcaac7b289a198fbad58001af82cc9edbbc8`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e7d61bc03c6ee6237c30fc72d8e78f9ae68806cc5a2cf46b7656b4b20eee7fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202799730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d1150fcdbed35bf916de083686b185418c1e6a6899a3b61c1b50d0803144fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:27:15 GMT
ENV RUBY_MAJOR=2.7
# Wed, 13 Oct 2021 17:27:16 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 13 Oct 2021 17:27:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 13 Oct 2021 17:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:28:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:28:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:28:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:07:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:07:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:07:32 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:07:33 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:07:34 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:07:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:07:36 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 18:07:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 18:07:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:10:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:10:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:10:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:10:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:10:14 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:10:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e838a1f60b724d27421dc669bb812af64671ae1601d8730a909695f985a9853`  
		Last Modified: Wed, 13 Oct 2021 17:49:43 GMT  
		Size: 14.1 MB (14143875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963345e088e83677ac3681509027812db0797dd4e631453708af27bbb7645249`  
		Last Modified: Wed, 13 Oct 2021 17:49:41 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394c6771c31ed3bd4fb7c995c8386bec3486e771e2dfa0681f7c5ea822bb971`  
		Last Modified: Wed, 13 Oct 2021 18:16:19 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da764cc87fa4bae907bda083490a29da7979cadd80814f5f362363a376593464`  
		Last Modified: Wed, 13 Oct 2021 18:16:50 GMT  
		Size: 92.6 MB (92615308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3a357444ace950e06fd5b35b20936a1a04a878a138b079900a2a4e02d62a3`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291526f865480d0636e29e2568a193613d43500bc8436edc5155cba7be88cae5`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276061b01ba9d6d30524f2fe777d3cec8be623bcfe6dab6b1c508872ddda38a9`  
		Last Modified: Wed, 13 Oct 2021 18:16:18 GMT  
		Size: 3.1 MB (3063380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75cc333a34f7788294e590abc79600965f6cf2d3f8561dbed33adc0362fd0c`  
		Last Modified: Wed, 13 Oct 2021 18:16:23 GMT  
		Size: 55.8 MB (55802879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d0466145763c731bdea690ba220239abbd35ca06ab4a5aa668c8e5b1510315`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:343086eb10fea1d0e294d959366776bd9cd3527c2b8f78ca2b41a25ce57f7c04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202133811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf5f72b35bd546cc8491264dba7674efb2a02f82fb9dea6db538ed870c4522b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 16:03:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:03:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:03:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:03:51 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:41:44 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:42:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:42:47 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:42:48 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:42:48 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:42:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:42:51 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:42:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:42:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:44:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:44:45 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:44:45 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:44:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:44:46 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:44:46 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba726e6e9acd11bec848488e1d9ba1dd28603662a05cb961c478edf2dfb5897b`  
		Last Modified: Tue, 12 Oct 2021 16:23:37 GMT  
		Size: 14.0 MB (13992252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfdcccd0ac8347312f70337b19af20dff7404116557f68a2ecddf40d033a66`  
		Last Modified: Tue, 12 Oct 2021 16:23:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d43d0920022abbdbd2439bdbfc251a541a3312219812894a15104cbc36da451`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c9895082195c18acb3a1950bccbfb998972a2a19b629d0e896b63ff2e9786c`  
		Last Modified: Wed, 13 Oct 2021 03:53:03 GMT  
		Size: 95.7 MB (95702557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fdcdc153d4a0f4d19f41c12cb4136e6879e01aae4b46e54ccd246aacf8509`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2705eeb2a9eaf702125ec2c318782eb4f43d41117ac7c7f2dab36275112d0b3`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb661f169d61250b0e2722b5df44b38e86dfe23c77a7d89e2871f7067e6b1e7`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 3.1 MB (3063242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143e4562d00275914a9d8cc6aad9335737e0bafde273ef01ce97c216fb8d73bd`  
		Last Modified: Wed, 13 Oct 2021 03:52:39 GMT  
		Size: 44.4 MB (44353070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4cf1b02b914b02976906375ae2c1c362060af22baccb8ed548f6a40b930399`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:a4c48b2c0bbb76d20734a3239c5ff4486fb06902d9161041f74716b4da26ab4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219642463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21372e7251d350b037972153cf0703df9289044566d5c57094d019c86f77787`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 18:52:55 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 18:53:00 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 18:53:05 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 18:59:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 18:59:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 18:59:55 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:46:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:46:53 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:46:59 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:47:04 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:47:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:47:21 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 14 Oct 2021 00:47:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 14 Oct 2021 00:47:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 00:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 00:52:57 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 00:53:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 00:53:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 00:53:25 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 00:53:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421cf7b60e6ecf3d6ad60b357e419014d8f6ad271c958a247f07c42e24664d11`  
		Last Modified: Tue, 12 Oct 2021 19:32:25 GMT  
		Size: 15.0 MB (14997040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06540a2f04ef35b100c723361f0086cb3542d114ee0eea90d820e05137d9c5dc`  
		Last Modified: Tue, 12 Oct 2021 19:32:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718e7a16edeab031c20f2c31cd9a6f1421c88037a4dfcf8b59604f89539cd11`  
		Last Modified: Thu, 14 Oct 2021 01:20:37 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a889dd8c5dd31d494ac35831e782d265b2bfe457db83677f7c047312896493`  
		Last Modified: Thu, 14 Oct 2021 01:21:41 GMT  
		Size: 101.3 MB (101327529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca7ef034d38ef39e783753bbb082ce26ec6fdd002cf9a68ce51058795ad8573`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232465c4db3849de029290c3113d2e54c170959078f1c6db79be04f25679d9`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ee5c28f159c990af395a85aca6dd92d3e5df1db87f1d1b22dd971db191ffa0`  
		Last Modified: Thu, 14 Oct 2021 01:20:33 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea081b840509c49626aada5a751b15f06425894b1909de76d192b435f459d`  
		Last Modified: Thu, 14 Oct 2021 01:20:40 GMT  
		Size: 57.0 MB (56997726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af764c7ef4e285b105b1dfdd393764172a828c880727596371b3d095e4fcd5`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; s390x

```console
$ docker pull redmine@sha256:2d2e87d503c62c577e846a38406e5c4a17b470e0aff9daa3d535ad926ed37084
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202563722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a0171ae100a0cc3078e21c5b0bc20844d39c2bcebcf79ca3c96a0dc2c81552`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 04:18:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:18:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:18:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:18:07 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:35:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:36:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:36:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:36:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:36:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:36:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 09:36:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:38:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:38:07 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:38:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:38:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:38:07 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:38:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5683829b72e9a4d66e64d82641db943f6743e6c70a9a696d5ecee3d2bf6d2b5f`  
		Last Modified: Tue, 12 Oct 2021 04:31:02 GMT  
		Size: 14.7 MB (14697069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe5e8ef560af46263eb3ebe0e4907eeec84b5f7449bda56fd1cc07f5d84e234`  
		Last Modified: Tue, 12 Oct 2021 04:31:00 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b986a39650e8c61b28fb2e7aad4c6967ee7053443d5dd0f238431e9df00ed`  
		Last Modified: Tue, 12 Oct 2021 09:44:01 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e60616cc73d3b71b45dd0abf5d150c14c873b71026a5d817bb84fe76d32df5`  
		Last Modified: Tue, 12 Oct 2021 09:44:13 GMT  
		Size: 91.8 MB (91790121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a5fe3e5668c6414afc329a80c0981f446460312ec614052ea55a4b08d7e46f`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8ac8ca9b149047ed48dcb25ad3be07111b971715f73d0375a395b3a27af965`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960d15f81c4c390cd09bd901489ce0b96bbccda8a5f2bcd15f0243ae2df9d99`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25229088271a14206c72d9bf135c45e47af738e5da50cee70fd9d1821500b547`  
		Last Modified: Tue, 12 Oct 2021 09:44:04 GMT  
		Size: 56.4 MB (56439455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d605facdd969ae1f1091b22c319f219b199e11c31a4a879a23d7fe92d50d8307`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:cf4ec4d559c84d289809ddc6554057e6522d3720200a340c70ba098c12202c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:518ba4effd92c427ef19922743eea649ed001436d8a66fe0de469abb2de00949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149044368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48a04de41bf1795abeee36effc817551b3de5069209d3ec827816281c81211a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_MAJOR=2.7
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 13 Nov 2021 06:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 13 Nov 2021 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:47:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:47:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:47:56 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:28:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:29:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:29:07 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:29:08 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:29:08 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_VERSION=4.2.3
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Sat, 13 Nov 2021 14:29:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:29:13 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:31:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:31:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:31:22 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:31:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81c0605571c3961987ae1ce872ebef2b5bcb439010c194e90b47282556c32d`  
		Last Modified: Sat, 13 Nov 2021 06:58:25 GMT  
		Size: 14.0 MB (13994126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2814005984530d27bc89e1c810fb8cb01371038a28bc3d85a1e95b710d9e043e`  
		Last Modified: Sat, 13 Nov 2021 06:58:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171914095295d927972128e1f66156ce389cb697d40fc6d7ea68c919861015e`  
		Last Modified: Sat, 13 Nov 2021 14:36:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9802858485f172f49a49aa23ebc2ef97aa9a7dff598d4d6b18f27e107ae24436`  
		Last Modified: Sat, 13 Nov 2021 14:36:55 GMT  
		Size: 69.5 MB (69548252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5b29e3b352df46dbdcf96478507ab2ace06abee4b91e86cea6852a73067d98`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd79647c11e0ebdbaa7b41c71d969403768f7950e69f1b9eda5545fe42e86b3`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20504c29a1f01e91c83c2e1e82a90fb05c118bbf74d44fa621ec588a179bce4b`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 3.1 MB (3064272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d43b9df6162fdd2b107724ff288c851a49738e7e04fa16cd34fddde661b04`  
		Last Modified: Sat, 13 Nov 2021 14:36:48 GMT  
		Size: 56.0 MB (56029256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561c4b4d66001dcdc5ff09131812075d6a6d4f6430e175565724033921e826f1`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-passenger`

```console
$ docker pull redmine@sha256:0a2beba76e007d174f23a2648bb6286f22d459f02c4e52c079b233cc06019f18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:5df4cc2cc1a71f5966a962dabe733bb283f5dcf2d5d79c9a624ca4d234f974b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221663528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88e23cfd35a24f595790cf1434facb584b62ba6518a62473675f114c5bed8f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:11 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:46:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:46:36 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:46:36 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:46:36 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284a323be9f6611677ab116846d6c4dbf712313bcce34cf3e2c684501d18e10`  
		Last Modified: Wed, 10 Nov 2021 03:48:08 GMT  
		Size: 21.2 MB (21238255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebe82b2f5ac28b2b6826a4aec1e29a72892ccea15a741fc388f2c686094da69`  
		Last Modified: Wed, 10 Nov 2021 03:48:06 GMT  
		Size: 4.9 MB (4924623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.3`

```console
$ docker pull redmine@sha256:75c11d669206fefdb4e833f087be5a76327fe402ebda35ac41880656cf9c2128
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

### `redmine:4.2.3` - linux; amd64

```console
$ docker pull redmine@sha256:23da6bbd8146ba5ebc6c565af6a4941d0a836fb5f2b3cf8281d954a84047c675
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195500650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777ff92e6fdbdb00a6ebcf1c2df29c52c4cbb171e418bcee49451b9df8ddf3b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; arm variant v5

```console
$ docker pull redmine@sha256:08f124ad97cbf3d78e62b390897fbd0a6e47f4901f4ce4f632d68de47d1236c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196991904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750dc7fdc53efaea0a675c5102c8cc3d6c8e5fb47e2bb056eae33416edf86f72`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 07:03:18 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 07:07:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:07:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:07:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:07:39 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:06:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:06:17 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:06:19 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:06:20 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:06:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:06:24 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:06:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:06:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:13:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:13:17 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:13:19 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:13:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:13:22 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854afe8d48105a800902d829046a9890cab76441d450aa59877c28405734daed`  
		Last Modified: Tue, 12 Oct 2021 07:33:59 GMT  
		Size: 13.9 MB (13871429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97d908af060f6e00c4e7a607087a50b553e21e08c6a8c70274a3d81ea0b3ef`  
		Last Modified: Tue, 12 Oct 2021 07:33:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a08bb1308b5863e00403e1a34c4cb2a9aafa57091f2d1faa4936463e4f8de79`  
		Last Modified: Wed, 13 Oct 2021 03:32:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b177e5e016cce70192ebf1277d5a21559c74cf5aa60e6bff5dfb31a9d5767e8`  
		Last Modified: Wed, 13 Oct 2021 03:32:45 GMT  
		Size: 89.6 MB (89577077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa429c867c2a22535e2c33e168d8de14f69c6f13124dc7494d06630528d03c43`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168fe406bb1360b18d49546d4af05cccf7fb548d99e4f4663d83dab19f23f4be`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2ee921f4dfd9c1a73cfe3b44b39e67f1af385494dd03e3fe1cbdc9c31aaf1`  
		Last Modified: Wed, 13 Oct 2021 03:32:04 GMT  
		Size: 3.1 MB (3063249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892b495be3664dd078f8510b6b3222fec0b0eeceaaa8fcc540d7ced595ecf23`  
		Last Modified: Wed, 13 Oct 2021 03:32:21 GMT  
		Size: 55.3 MB (55253893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea12a2e245bbbc4585eb36f1a1709b9035c2beaac9e1be72d14f2bf9c84118e`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; arm variant v7

```console
$ docker pull redmine@sha256:900b0cad4acc6dc28f8f9e3279e4a10121c4d247bd540f66d7ff40fcdf914200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190138732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88b04a543401c43e354aa169b439ad085b11a2b6acbde3b9a6a36f4307bec08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 03:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:10:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:10:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:10:57 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:34:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:35:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:35:44 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:35:45 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:35:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:35:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:35:48 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 06:35:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 06:35:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:41:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:41:11 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:41:12 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:41:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ab36f90d94f50bb2f0b4be72799049691d9d0f05aadbe4e5cba89a3989efd1`  
		Last Modified: Tue, 12 Oct 2021 03:41:56 GMT  
		Size: 13.8 MB (13767235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a22941e2b0ce8584f2fa791a8370a30bd3a202fa73a1dd64d00a85bf075916a`  
		Last Modified: Tue, 12 Oct 2021 03:41:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6828dc1bb7b47f9d60169ee81885096702049306577ce953096d5057c12e91af`  
		Last Modified: Wed, 13 Oct 2021 06:55:56 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e9962d77928a7fea0f4dd24c838a24f72da3eba59ed75e59a3557633655398`  
		Last Modified: Wed, 13 Oct 2021 06:56:52 GMT  
		Size: 85.6 MB (85590281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894593e78f4567729a26e4302a660a56ee7289a18398fb9ec5b526be2466b739`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f705a0b143059f649ff99fd7d343002386794bfe675456f393697b71d9dbc5`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14825a50627a0f65eec1cc695fb3896ea4d8a22a09fc112bc902fcbbdd53be02`  
		Last Modified: Wed, 13 Oct 2021 06:56:03 GMT  
		Size: 3.1 MB (3063246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461661b0c3351479c43855bab9a39d5482ee87a52376bc2898c48b83ce9ada1`  
		Last Modified: Wed, 13 Oct 2021 06:56:20 GMT  
		Size: 55.1 MB (55101134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b2c0757c967dd445d6615d9fa9fcaac7b289a198fbad58001af82cc9edbbc8`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e7d61bc03c6ee6237c30fc72d8e78f9ae68806cc5a2cf46b7656b4b20eee7fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202799730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d1150fcdbed35bf916de083686b185418c1e6a6899a3b61c1b50d0803144fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:27:15 GMT
ENV RUBY_MAJOR=2.7
# Wed, 13 Oct 2021 17:27:16 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 13 Oct 2021 17:27:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 13 Oct 2021 17:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:28:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:28:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:28:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:07:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:07:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:07:32 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:07:33 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:07:34 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:07:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:07:36 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 18:07:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 18:07:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:10:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:10:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:10:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:10:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:10:14 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:10:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e838a1f60b724d27421dc669bb812af64671ae1601d8730a909695f985a9853`  
		Last Modified: Wed, 13 Oct 2021 17:49:43 GMT  
		Size: 14.1 MB (14143875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963345e088e83677ac3681509027812db0797dd4e631453708af27bbb7645249`  
		Last Modified: Wed, 13 Oct 2021 17:49:41 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394c6771c31ed3bd4fb7c995c8386bec3486e771e2dfa0681f7c5ea822bb971`  
		Last Modified: Wed, 13 Oct 2021 18:16:19 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da764cc87fa4bae907bda083490a29da7979cadd80814f5f362363a376593464`  
		Last Modified: Wed, 13 Oct 2021 18:16:50 GMT  
		Size: 92.6 MB (92615308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3a357444ace950e06fd5b35b20936a1a04a878a138b079900a2a4e02d62a3`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291526f865480d0636e29e2568a193613d43500bc8436edc5155cba7be88cae5`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276061b01ba9d6d30524f2fe777d3cec8be623bcfe6dab6b1c508872ddda38a9`  
		Last Modified: Wed, 13 Oct 2021 18:16:18 GMT  
		Size: 3.1 MB (3063380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75cc333a34f7788294e590abc79600965f6cf2d3f8561dbed33adc0362fd0c`  
		Last Modified: Wed, 13 Oct 2021 18:16:23 GMT  
		Size: 55.8 MB (55802879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d0466145763c731bdea690ba220239abbd35ca06ab4a5aa668c8e5b1510315`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; 386

```console
$ docker pull redmine@sha256:343086eb10fea1d0e294d959366776bd9cd3527c2b8f78ca2b41a25ce57f7c04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202133811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf5f72b35bd546cc8491264dba7674efb2a02f82fb9dea6db538ed870c4522b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 16:03:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:03:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:03:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:03:51 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:41:44 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:42:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:42:47 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:42:48 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:42:48 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:42:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:42:51 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:42:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:42:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:44:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:44:45 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:44:45 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:44:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:44:46 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:44:46 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba726e6e9acd11bec848488e1d9ba1dd28603662a05cb961c478edf2dfb5897b`  
		Last Modified: Tue, 12 Oct 2021 16:23:37 GMT  
		Size: 14.0 MB (13992252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfdcccd0ac8347312f70337b19af20dff7404116557f68a2ecddf40d033a66`  
		Last Modified: Tue, 12 Oct 2021 16:23:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d43d0920022abbdbd2439bdbfc251a541a3312219812894a15104cbc36da451`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c9895082195c18acb3a1950bccbfb998972a2a19b629d0e896b63ff2e9786c`  
		Last Modified: Wed, 13 Oct 2021 03:53:03 GMT  
		Size: 95.7 MB (95702557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fdcdc153d4a0f4d19f41c12cb4136e6879e01aae4b46e54ccd246aacf8509`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2705eeb2a9eaf702125ec2c318782eb4f43d41117ac7c7f2dab36275112d0b3`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb661f169d61250b0e2722b5df44b38e86dfe23c77a7d89e2871f7067e6b1e7`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 3.1 MB (3063242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143e4562d00275914a9d8cc6aad9335737e0bafde273ef01ce97c216fb8d73bd`  
		Last Modified: Wed, 13 Oct 2021 03:52:39 GMT  
		Size: 44.4 MB (44353070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4cf1b02b914b02976906375ae2c1c362060af22baccb8ed548f6a40b930399`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; ppc64le

```console
$ docker pull redmine@sha256:a4c48b2c0bbb76d20734a3239c5ff4486fb06902d9161041f74716b4da26ab4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219642463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21372e7251d350b037972153cf0703df9289044566d5c57094d019c86f77787`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 18:52:55 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 18:53:00 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 18:53:05 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 18:59:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 18:59:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 18:59:55 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:46:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:46:53 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:46:59 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:47:04 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:47:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:47:21 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 14 Oct 2021 00:47:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 14 Oct 2021 00:47:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 00:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 00:52:57 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 00:53:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 00:53:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 00:53:25 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 00:53:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421cf7b60e6ecf3d6ad60b357e419014d8f6ad271c958a247f07c42e24664d11`  
		Last Modified: Tue, 12 Oct 2021 19:32:25 GMT  
		Size: 15.0 MB (14997040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06540a2f04ef35b100c723361f0086cb3542d114ee0eea90d820e05137d9c5dc`  
		Last Modified: Tue, 12 Oct 2021 19:32:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718e7a16edeab031c20f2c31cd9a6f1421c88037a4dfcf8b59604f89539cd11`  
		Last Modified: Thu, 14 Oct 2021 01:20:37 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a889dd8c5dd31d494ac35831e782d265b2bfe457db83677f7c047312896493`  
		Last Modified: Thu, 14 Oct 2021 01:21:41 GMT  
		Size: 101.3 MB (101327529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca7ef034d38ef39e783753bbb082ce26ec6fdd002cf9a68ce51058795ad8573`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232465c4db3849de029290c3113d2e54c170959078f1c6db79be04f25679d9`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ee5c28f159c990af395a85aca6dd92d3e5df1db87f1d1b22dd971db191ffa0`  
		Last Modified: Thu, 14 Oct 2021 01:20:33 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea081b840509c49626aada5a751b15f06425894b1909de76d192b435f459d`  
		Last Modified: Thu, 14 Oct 2021 01:20:40 GMT  
		Size: 57.0 MB (56997726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af764c7ef4e285b105b1dfdd393764172a828c880727596371b3d095e4fcd5`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.3` - linux; s390x

```console
$ docker pull redmine@sha256:2d2e87d503c62c577e846a38406e5c4a17b470e0aff9daa3d535ad926ed37084
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202563722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a0171ae100a0cc3078e21c5b0bc20844d39c2bcebcf79ca3c96a0dc2c81552`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 04:18:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:18:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:18:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:18:07 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:35:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:36:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:36:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:36:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:36:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:36:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 09:36:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:38:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:38:07 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:38:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:38:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:38:07 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:38:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5683829b72e9a4d66e64d82641db943f6743e6c70a9a696d5ecee3d2bf6d2b5f`  
		Last Modified: Tue, 12 Oct 2021 04:31:02 GMT  
		Size: 14.7 MB (14697069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe5e8ef560af46263eb3ebe0e4907eeec84b5f7449bda56fd1cc07f5d84e234`  
		Last Modified: Tue, 12 Oct 2021 04:31:00 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b986a39650e8c61b28fb2e7aad4c6967ee7053443d5dd0f238431e9df00ed`  
		Last Modified: Tue, 12 Oct 2021 09:44:01 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e60616cc73d3b71b45dd0abf5d150c14c873b71026a5d817bb84fe76d32df5`  
		Last Modified: Tue, 12 Oct 2021 09:44:13 GMT  
		Size: 91.8 MB (91790121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a5fe3e5668c6414afc329a80c0981f446460312ec614052ea55a4b08d7e46f`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8ac8ca9b149047ed48dcb25ad3be07111b971715f73d0375a395b3a27af965`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960d15f81c4c390cd09bd901489ce0b96bbccda8a5f2bcd15f0243ae2df9d99`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25229088271a14206c72d9bf135c45e47af738e5da50cee70fd9d1821500b547`  
		Last Modified: Tue, 12 Oct 2021 09:44:04 GMT  
		Size: 56.4 MB (56439455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d605facdd969ae1f1091b22c319f219b199e11c31a4a879a23d7fe92d50d8307`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.3-alpine`

```console
$ docker pull redmine@sha256:cf4ec4d559c84d289809ddc6554057e6522d3720200a340c70ba098c12202c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.3-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:518ba4effd92c427ef19922743eea649ed001436d8a66fe0de469abb2de00949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149044368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48a04de41bf1795abeee36effc817551b3de5069209d3ec827816281c81211a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_MAJOR=2.7
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 13 Nov 2021 06:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 13 Nov 2021 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:47:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:47:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:47:56 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:28:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:29:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:29:07 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:29:08 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:29:08 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_VERSION=4.2.3
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Sat, 13 Nov 2021 14:29:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:29:13 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:31:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:31:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:31:22 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:31:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81c0605571c3961987ae1ce872ebef2b5bcb439010c194e90b47282556c32d`  
		Last Modified: Sat, 13 Nov 2021 06:58:25 GMT  
		Size: 14.0 MB (13994126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2814005984530d27bc89e1c810fb8cb01371038a28bc3d85a1e95b710d9e043e`  
		Last Modified: Sat, 13 Nov 2021 06:58:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171914095295d927972128e1f66156ce389cb697d40fc6d7ea68c919861015e`  
		Last Modified: Sat, 13 Nov 2021 14:36:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9802858485f172f49a49aa23ebc2ef97aa9a7dff598d4d6b18f27e107ae24436`  
		Last Modified: Sat, 13 Nov 2021 14:36:55 GMT  
		Size: 69.5 MB (69548252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5b29e3b352df46dbdcf96478507ab2ace06abee4b91e86cea6852a73067d98`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd79647c11e0ebdbaa7b41c71d969403768f7950e69f1b9eda5545fe42e86b3`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20504c29a1f01e91c83c2e1e82a90fb05c118bbf74d44fa621ec588a179bce4b`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 3.1 MB (3064272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d43b9df6162fdd2b107724ff288c851a49738e7e04fa16cd34fddde661b04`  
		Last Modified: Sat, 13 Nov 2021 14:36:48 GMT  
		Size: 56.0 MB (56029256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561c4b4d66001dcdc5ff09131812075d6a6d4f6430e175565724033921e826f1`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.3-passenger`

```console
$ docker pull redmine@sha256:0a2beba76e007d174f23a2648bb6286f22d459f02c4e52c079b233cc06019f18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:5df4cc2cc1a71f5966a962dabe733bb283f5dcf2d5d79c9a624ca4d234f974b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221663528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88e23cfd35a24f595790cf1434facb584b62ba6518a62473675f114c5bed8f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:11 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:46:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:46:36 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:46:36 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:46:36 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284a323be9f6611677ab116846d6c4dbf712313bcce34cf3e2c684501d18e10`  
		Last Modified: Wed, 10 Nov 2021 03:48:08 GMT  
		Size: 21.2 MB (21238255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebe82b2f5ac28b2b6826a4aec1e29a72892ccea15a741fc388f2c686094da69`  
		Last Modified: Wed, 10 Nov 2021 03:48:06 GMT  
		Size: 4.9 MB (4924623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:cf4ec4d559c84d289809ddc6554057e6522d3720200a340c70ba098c12202c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:518ba4effd92c427ef19922743eea649ed001436d8a66fe0de469abb2de00949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149044368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48a04de41bf1795abeee36effc817551b3de5069209d3ec827816281c81211a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_MAJOR=2.7
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 13 Nov 2021 06:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 13 Nov 2021 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:47:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:47:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:47:56 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:28:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:29:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:29:07 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:29:08 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:29:08 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_VERSION=4.2.3
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Sat, 13 Nov 2021 14:29:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:29:13 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:31:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:31:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:31:22 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:31:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81c0605571c3961987ae1ce872ebef2b5bcb439010c194e90b47282556c32d`  
		Last Modified: Sat, 13 Nov 2021 06:58:25 GMT  
		Size: 14.0 MB (13994126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2814005984530d27bc89e1c810fb8cb01371038a28bc3d85a1e95b710d9e043e`  
		Last Modified: Sat, 13 Nov 2021 06:58:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171914095295d927972128e1f66156ce389cb697d40fc6d7ea68c919861015e`  
		Last Modified: Sat, 13 Nov 2021 14:36:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9802858485f172f49a49aa23ebc2ef97aa9a7dff598d4d6b18f27e107ae24436`  
		Last Modified: Sat, 13 Nov 2021 14:36:55 GMT  
		Size: 69.5 MB (69548252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5b29e3b352df46dbdcf96478507ab2ace06abee4b91e86cea6852a73067d98`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd79647c11e0ebdbaa7b41c71d969403768f7950e69f1b9eda5545fe42e86b3`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20504c29a1f01e91c83c2e1e82a90fb05c118bbf74d44fa621ec588a179bce4b`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 3.1 MB (3064272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d43b9df6162fdd2b107724ff288c851a49738e7e04fa16cd34fddde661b04`  
		Last Modified: Sat, 13 Nov 2021 14:36:48 GMT  
		Size: 56.0 MB (56029256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561c4b4d66001dcdc5ff09131812075d6a6d4f6430e175565724033921e826f1`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:75c11d669206fefdb4e833f087be5a76327fe402ebda35ac41880656cf9c2128
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

### `redmine:latest` - linux; amd64

```console
$ docker pull redmine@sha256:23da6bbd8146ba5ebc6c565af6a4941d0a836fb5f2b3cf8281d954a84047c675
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195500650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777ff92e6fdbdb00a6ebcf1c2df29c52c4cbb171e418bcee49451b9df8ddf3b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:08f124ad97cbf3d78e62b390897fbd0a6e47f4901f4ce4f632d68de47d1236c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196991904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750dc7fdc53efaea0a675c5102c8cc3d6c8e5fb47e2bb056eae33416edf86f72`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:51:32 GMT
ADD file:0d95eee31ffe3f4260263e4fac2a61123a4b98d2e7a67efcc7bfea338c54f41d in / 
# Tue, 12 Oct 2021 00:51:32 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:45:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 06:45:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 06:45:07 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 07:03:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 07:03:18 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 07:07:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 07:07:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 07:07:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 07:07:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 07:07:39 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:06:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:06:17 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:06:19 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:06:20 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:06:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:06:24 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:06:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:06:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:13:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:13:17 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:13:19 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:13:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:13:22 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:175b083b22fb061f7d1894fe4916a2967ce636d47376da526d90d57c8f7efc60`  
		Last Modified: Tue, 12 Oct 2021 01:07:45 GMT  
		Size: 24.9 MB (24872704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed73113a2340f22427741647a89a1911c6dd067bde17833928c5d210ab93918`  
		Last Modified: Tue, 12 Oct 2021 07:31:54 GMT  
		Size: 10.3 MB (10349314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7a78f939d570718e0af30429b3118d94e3800937a469b3fca591fda6d0540e`  
		Last Modified: Tue, 12 Oct 2021 07:31:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854afe8d48105a800902d829046a9890cab76441d450aa59877c28405734daed`  
		Last Modified: Tue, 12 Oct 2021 07:33:59 GMT  
		Size: 13.9 MB (13871429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc97d908af060f6e00c4e7a607087a50b553e21e08c6a8c70274a3d81ea0b3ef`  
		Last Modified: Tue, 12 Oct 2021 07:33:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a08bb1308b5863e00403e1a34c4cb2a9aafa57091f2d1faa4936463e4f8de79`  
		Last Modified: Wed, 13 Oct 2021 03:32:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b177e5e016cce70192ebf1277d5a21559c74cf5aa60e6bff5dfb31a9d5767e8`  
		Last Modified: Wed, 13 Oct 2021 03:32:45 GMT  
		Size: 89.6 MB (89577077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa429c867c2a22535e2c33e168d8de14f69c6f13124dc7494d06630528d03c43`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168fe406bb1360b18d49546d4af05cccf7fb548d99e4f4663d83dab19f23f4be`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec2ee921f4dfd9c1a73cfe3b44b39e67f1af385494dd03e3fe1cbdc9c31aaf1`  
		Last Modified: Wed, 13 Oct 2021 03:32:04 GMT  
		Size: 3.1 MB (3063249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7892b495be3664dd078f8510b6b3222fec0b0eeceaaa8fcc540d7ced595ecf23`  
		Last Modified: Wed, 13 Oct 2021 03:32:21 GMT  
		Size: 55.3 MB (55253893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea12a2e245bbbc4585eb36f1a1709b9035c2beaac9e1be72d14f2bf9c84118e`  
		Last Modified: Wed, 13 Oct 2021 03:32:01 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:900b0cad4acc6dc28f8f9e3279e4a10121c4d247bd540f66d7ff40fcdf914200
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190138732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88b04a543401c43e354aa169b439ad085b11a2b6acbde3b9a6a36f4307bec08`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:56:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:56:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 02:56:30 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 03:06:47 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 03:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 03:10:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 03:10:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 03:10:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 03:10:57 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 06:34:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 06:35:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:35:44 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 06:35:45 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 06:35:46 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 06:35:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 06:35:48 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 06:35:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 06:35:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 06:41:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 06:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 06:41:11 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 06:41:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 06:41:12 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 06:41:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd321094894b78bc0792d96cf339ee9e4ce7ec18a14ea44b32cfbc809867b`  
		Last Modified: Tue, 12 Oct 2021 03:40:20 GMT  
		Size: 9.9 MB (9872904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0e1a382b6eb02d552bdb97946d22f8b0d9b5f787b5d1b491fa3703e23d5ea`  
		Last Modified: Tue, 12 Oct 2021 03:40:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ab36f90d94f50bb2f0b4be72799049691d9d0f05aadbe4e5cba89a3989efd1`  
		Last Modified: Tue, 12 Oct 2021 03:41:56 GMT  
		Size: 13.8 MB (13767235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a22941e2b0ce8584f2fa791a8370a30bd3a202fa73a1dd64d00a85bf075916a`  
		Last Modified: Tue, 12 Oct 2021 03:41:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6828dc1bb7b47f9d60169ee81885096702049306577ce953096d5057c12e91af`  
		Last Modified: Wed, 13 Oct 2021 06:55:56 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e9962d77928a7fea0f4dd24c838a24f72da3eba59ed75e59a3557633655398`  
		Last Modified: Wed, 13 Oct 2021 06:56:52 GMT  
		Size: 85.6 MB (85590281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894593e78f4567729a26e4302a660a56ee7289a18398fb9ec5b526be2466b739`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f705a0b143059f649ff99fd7d343002386794bfe675456f393697b71d9dbc5`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14825a50627a0f65eec1cc695fb3896ea4d8a22a09fc112bc902fcbbdd53be02`  
		Last Modified: Wed, 13 Oct 2021 06:56:03 GMT  
		Size: 3.1 MB (3063246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f461661b0c3351479c43855bab9a39d5482ee87a52376bc2898c48b83ce9ada1`  
		Last Modified: Wed, 13 Oct 2021 06:56:20 GMT  
		Size: 55.1 MB (55101134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b2c0757c967dd445d6615d9fa9fcaac7b289a198fbad58001af82cc9edbbc8`  
		Last Modified: Wed, 13 Oct 2021 06:55:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e7d61bc03c6ee6237c30fc72d8e78f9ae68806cc5a2cf46b7656b4b20eee7fdc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202799730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d1150fcdbed35bf916de083686b185418c1e6a6899a3b61c1b50d0803144fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 17:14:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 17:14:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Oct 2021 17:14:43 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 17:27:15 GMT
ENV RUBY_MAJOR=2.7
# Wed, 13 Oct 2021 17:27:16 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 13 Oct 2021 17:27:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 13 Oct 2021 17:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Oct 2021 17:28:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Oct 2021 17:28:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 17:28:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Oct 2021 17:28:59 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 18:07:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 18:07:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 18:07:32 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 18:07:33 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 18:07:34 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 18:07:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 18:07:36 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 18:07:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 18:07:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 18:10:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 18:10:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 18:10:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 18:10:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 18:10:14 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 18:10:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92d13d4e13323ab4d34f4ea73bd0f9f167c72e753b2297d168646ac29a70cfe`  
		Last Modified: Wed, 13 Oct 2021 17:47:26 GMT  
		Size: 11.3 MB (11261779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a304271b5865f80f88114a169c832cc685d86951ea38b7d071469ca15ab9cc75`  
		Last Modified: Wed, 13 Oct 2021 17:47:24 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e838a1f60b724d27421dc669bb812af64671ae1601d8730a909695f985a9853`  
		Last Modified: Wed, 13 Oct 2021 17:49:43 GMT  
		Size: 14.1 MB (14143875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963345e088e83677ac3681509027812db0797dd4e631453708af27bbb7645249`  
		Last Modified: Wed, 13 Oct 2021 17:49:41 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394c6771c31ed3bd4fb7c995c8386bec3486e771e2dfa0681f7c5ea822bb971`  
		Last Modified: Wed, 13 Oct 2021 18:16:19 GMT  
		Size: 1.6 KB (1626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da764cc87fa4bae907bda083490a29da7979cadd80814f5f362363a376593464`  
		Last Modified: Wed, 13 Oct 2021 18:16:50 GMT  
		Size: 92.6 MB (92615308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3a357444ace950e06fd5b35b20936a1a04a878a138b079900a2a4e02d62a3`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291526f865480d0636e29e2568a193613d43500bc8436edc5155cba7be88cae5`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276061b01ba9d6d30524f2fe777d3cec8be623bcfe6dab6b1c508872ddda38a9`  
		Last Modified: Wed, 13 Oct 2021 18:16:18 GMT  
		Size: 3.1 MB (3063380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b75cc333a34f7788294e590abc79600965f6cf2d3f8561dbed33adc0362fd0c`  
		Last Modified: Wed, 13 Oct 2021 18:16:23 GMT  
		Size: 55.8 MB (55802879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d0466145763c731bdea690ba220239abbd35ca06ab4a5aa668c8e5b1510315`  
		Last Modified: Wed, 13 Oct 2021 18:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:343086eb10fea1d0e294d959366776bd9cd3527c2b8f78ca2b41a25ce57f7c04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202133811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf5f72b35bd546cc8491264dba7674efb2a02f82fb9dea6db538ed870c4522b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:47:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:47:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 16:00:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 16:03:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 16:03:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 16:03:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:03:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 16:03:51 GMT
CMD ["irb"]
# Wed, 13 Oct 2021 03:41:44 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 13 Oct 2021 03:42:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:42:47 GMT
ENV RAILS_ENV=production
# Wed, 13 Oct 2021 03:42:48 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Oct 2021 03:42:48 GMT
ENV HOME=/home/redmine
# Wed, 13 Oct 2021 03:42:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 13 Oct 2021 03:42:51 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 13 Oct 2021 03:42:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 13 Oct 2021 03:42:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 13 Oct 2021 03:44:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 13 Oct 2021 03:44:45 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 13 Oct 2021 03:44:45 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 13 Oct 2021 03:44:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 13 Oct 2021 03:44:46 GMT
EXPOSE 3000
# Wed, 13 Oct 2021 03:44:46 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb65f7fcc8ebb9e6545b6314cc3faf6b757da54c64b922a60de3d222d32f10`  
		Last Modified: Tue, 12 Oct 2021 16:21:54 GMT  
		Size: 17.2 MB (17227007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314af7a3bb5218705d63cdd25bc74924a835aa83d0e817bcd1591cf7c0e1797c`  
		Last Modified: Tue, 12 Oct 2021 16:21:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba726e6e9acd11bec848488e1d9ba1dd28603662a05cb961c478edf2dfb5897b`  
		Last Modified: Tue, 12 Oct 2021 16:23:37 GMT  
		Size: 14.0 MB (13992252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfdcccd0ac8347312f70337b19af20dff7404116557f68a2ecddf40d033a66`  
		Last Modified: Tue, 12 Oct 2021 16:23:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d43d0920022abbdbd2439bdbfc251a541a3312219812894a15104cbc36da451`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c9895082195c18acb3a1950bccbfb998972a2a19b629d0e896b63ff2e9786c`  
		Last Modified: Wed, 13 Oct 2021 03:53:03 GMT  
		Size: 95.7 MB (95702557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4fdcdc153d4a0f4d19f41c12cb4136e6879e01aae4b46e54ccd246aacf8509`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2705eeb2a9eaf702125ec2c318782eb4f43d41117ac7c7f2dab36275112d0b3`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb661f169d61250b0e2722b5df44b38e86dfe23c77a7d89e2871f7067e6b1e7`  
		Last Modified: Wed, 13 Oct 2021 03:52:27 GMT  
		Size: 3.1 MB (3063242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143e4562d00275914a9d8cc6aad9335737e0bafde273ef01ce97c216fb8d73bd`  
		Last Modified: Wed, 13 Oct 2021 03:52:39 GMT  
		Size: 44.4 MB (44353070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4cf1b02b914b02976906375ae2c1c362060af22baccb8ed548f6a40b930399`  
		Last Modified: Wed, 13 Oct 2021 03:52:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:a4c48b2c0bbb76d20734a3239c5ff4486fb06902d9161041f74716b4da26ab4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219642463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21372e7251d350b037972153cf0703df9289044566d5c57094d019c86f77787`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 01:26:46 GMT
ADD file:5526880c6f19a4b4231a8b2bd7cfc625d116764c4918eff6f0b55f8c1eb38e1a in / 
# Tue, 12 Oct 2021 01:26:50 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:23:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:24:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 18:24:11 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 18:52:55 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 18:53:00 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 18:53:05 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 18:59:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 18:59:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 18:59:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 18:59:55 GMT
CMD ["irb"]
# Thu, 14 Oct 2021 00:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 14 Oct 2021 00:46:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 00:46:53 GMT
ENV RAILS_ENV=production
# Thu, 14 Oct 2021 00:46:59 GMT
WORKDIR /usr/src/redmine
# Thu, 14 Oct 2021 00:47:04 GMT
ENV HOME=/home/redmine
# Thu, 14 Oct 2021 00:47:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 14 Oct 2021 00:47:21 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 14 Oct 2021 00:47:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 14 Oct 2021 00:47:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 14 Oct 2021 00:52:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 00:52:57 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 14 Oct 2021 00:53:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 14 Oct 2021 00:53:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 14 Oct 2021 00:53:25 GMT
EXPOSE 3000
# Thu, 14 Oct 2021 00:53:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d69973af32573c07c8789c0f9c144a5c0b822a1e85b59db3ce9f8ebc489ce85d`  
		Last Modified: Tue, 12 Oct 2021 01:38:40 GMT  
		Size: 30.5 MB (30547197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f48a596ad1fccd3e24dcc1f65e362937ced6f5b5ab61b6eb49e8eda8a55b85`  
		Last Modified: Tue, 12 Oct 2021 19:30:52 GMT  
		Size: 12.7 MB (12705483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd72e7e6250a90b152d1d27efca928b2c1bfc949dfe1b2e9cf089acde024c098`  
		Last Modified: Tue, 12 Oct 2021 19:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421cf7b60e6ecf3d6ad60b357e419014d8f6ad271c958a247f07c42e24664d11`  
		Last Modified: Tue, 12 Oct 2021 19:32:25 GMT  
		Size: 15.0 MB (14997040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06540a2f04ef35b100c723361f0086cb3542d114ee0eea90d820e05137d9c5dc`  
		Last Modified: Tue, 12 Oct 2021 19:32:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2718e7a16edeab031c20f2c31cd9a6f1421c88037a4dfcf8b59604f89539cd11`  
		Last Modified: Thu, 14 Oct 2021 01:20:37 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a889dd8c5dd31d494ac35831e782d265b2bfe457db83677f7c047312896493`  
		Last Modified: Thu, 14 Oct 2021 01:21:41 GMT  
		Size: 101.3 MB (101327529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca7ef034d38ef39e783753bbb082ce26ec6fdd002cf9a68ce51058795ad8573`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56232465c4db3849de029290c3113d2e54c170959078f1c6db79be04f25679d9`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ee5c28f159c990af395a85aca6dd92d3e5df1db87f1d1b22dd971db191ffa0`  
		Last Modified: Thu, 14 Oct 2021 01:20:33 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8ea081b840509c49626aada5a751b15f06425894b1909de76d192b435f459d`  
		Last Modified: Thu, 14 Oct 2021 01:20:40 GMT  
		Size: 57.0 MB (56997726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af764c7ef4e285b105b1dfdd393764172a828c880727596371b3d095e4fcd5`  
		Last Modified: Thu, 14 Oct 2021 01:20:32 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:2d2e87d503c62c577e846a38406e5c4a17b470e0aff9daa3d535ad926ed37084
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202563722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a0171ae100a0cc3078e21c5b0bc20844d39c2bcebcf79ca3c96a0dc2c81552`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:05:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:05:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 04:05:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 04:16:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 04:18:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 04:18:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 04:18:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 04:18:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 04:18:07 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 09:35:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 09:36:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:36:16 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 09:36:16 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 09:36:16 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 09:36:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 09:36:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 09:36:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 09:38:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 09:38:07 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 09:38:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 09:38:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:38:07 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 09:38:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152601da1f670f23930e38f542a251b56290100e816cebfc101161c8e9d9823`  
		Last Modified: Tue, 12 Oct 2021 04:30:27 GMT  
		Size: 10.8 MB (10815329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379c6f49f1643cab68ffcf8d485cf085a0799907e6458c13a589142d6763809`  
		Last Modified: Tue, 12 Oct 2021 04:30:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5683829b72e9a4d66e64d82641db943f6743e6c70a9a696d5ecee3d2bf6d2b5f`  
		Last Modified: Tue, 12 Oct 2021 04:31:02 GMT  
		Size: 14.7 MB (14697069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe5e8ef560af46263eb3ebe0e4907eeec84b5f7449bda56fd1cc07f5d84e234`  
		Last Modified: Tue, 12 Oct 2021 04:31:00 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5b986a39650e8c61b28fb2e7aad4c6967ee7053443d5dd0f238431e9df00ed`  
		Last Modified: Tue, 12 Oct 2021 09:44:01 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e60616cc73d3b71b45dd0abf5d150c14c873b71026a5d817bb84fe76d32df5`  
		Last Modified: Tue, 12 Oct 2021 09:44:13 GMT  
		Size: 91.8 MB (91790121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a5fe3e5668c6414afc329a80c0981f446460312ec614052ea55a4b08d7e46f`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8ac8ca9b149047ed48dcb25ad3be07111b971715f73d0375a395b3a27af965`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1960d15f81c4c390cd09bd901489ce0b96bbccda8a5f2bcd15f0243ae2df9d99`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 3.1 MB (3063245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25229088271a14206c72d9bf135c45e47af738e5da50cee70fd9d1821500b547`  
		Last Modified: Tue, 12 Oct 2021 09:44:04 GMT  
		Size: 56.4 MB (56439455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d605facdd969ae1f1091b22c319f219b199e11c31a4a879a23d7fe92d50d8307`  
		Last Modified: Tue, 12 Oct 2021 09:44:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:0a2beba76e007d174f23a2648bb6286f22d459f02c4e52c079b233cc06019f18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:5df4cc2cc1a71f5966a962dabe733bb283f5dcf2d5d79c9a624ca4d234f974b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221663528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88e23cfd35a24f595790cf1434facb584b62ba6518a62473675f114c5bed8f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:20:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:20:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Oct 2021 15:20:38 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 15:27:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 12 Oct 2021 15:27:25 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 12 Oct 2021 15:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Oct 2021 15:30:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Oct 2021 15:30:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 15:30:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Oct 2021 15:30:34 GMT
CMD ["irb"]
# Tue, 12 Oct 2021 20:17:43 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 12 Oct 2021 20:18:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:18:13 GMT
ENV RAILS_ENV=production
# Tue, 12 Oct 2021 20:18:13 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
ENV HOME=/home/redmine
# Tue, 12 Oct 2021 20:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:18:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 12 Oct 2021 20:18:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 12 Oct 2021 20:19:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Oct 2021 20:19:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Oct 2021 20:19:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 12 Oct 2021 20:19:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 20:19:21 GMT
EXPOSE 3000
# Tue, 12 Oct 2021 20:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 10 Nov 2021 03:46:11 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 10 Nov 2021 03:46:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 10 Nov 2021 03:46:36 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 10 Nov 2021 03:46:36 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 10 Nov 2021 03:46:36 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee6af487f217efc8e231b9857a8031fdf07ab0c8b30e539497893ec5287578b`  
		Last Modified: Tue, 12 Oct 2021 15:39:48 GMT  
		Size: 12.6 MB (12565186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48bb8449b0384f7addf4ec5d88d8ef088e25ca52f9299c1fca4bff3f5b2411d`  
		Last Modified: Tue, 12 Oct 2021 15:39:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4280126bdef2ed0df50609c224de8bcb7486f4ce6959104e588d7b147eb14f`  
		Last Modified: Tue, 12 Oct 2021 15:40:36 GMT  
		Size: 14.5 MB (14510184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4cc9067aac92ce406573f770322af2801a273925a95583e61e3ce6b568851a`  
		Last Modified: Tue, 12 Oct 2021 15:40:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf24873f395941528bd53ff8223d6b7799153cf8145e3b7158e496a8a4b9def`  
		Last Modified: Tue, 12 Oct 2021 20:27:17 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3deebb307eea15c0af224fa48dfa44ef5eb083d662d56e4eb24d97d503a2bb3f`  
		Last Modified: Tue, 12 Oct 2021 20:27:32 GMT  
		Size: 94.1 MB (94088542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799adc6ff62bdab4f48789fde71c3a76c4c1afa0e5288f175f5092a2e5867657`  
		Last Modified: Tue, 12 Oct 2021 20:27:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd34b5a0c4380ebac887ae883212d7ed6aa5e5fafbcfc5611ef03b072a3d34d`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b355bfb624ca195d5b52d9a3257d514eff56e8b581bfd705949d266e7e1cad4`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 3.1 MB (3063247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ccde718061b2b0d26691dacf79a140cd1b32f380e6c6d3a8f397be5156d44`  
		Last Modified: Tue, 12 Oct 2021 20:27:20 GMT  
		Size: 44.1 MB (44129736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e79252e1149fadd0907e406c69bd8e989028da830f9a410edb32ca9887a7d6`  
		Last Modified: Tue, 12 Oct 2021 20:27:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284a323be9f6611677ab116846d6c4dbf712313bcce34cf3e2c684501d18e10`  
		Last Modified: Wed, 10 Nov 2021 03:48:08 GMT  
		Size: 21.2 MB (21238255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebe82b2f5ac28b2b6826a4aec1e29a72892ccea15a741fc388f2c686094da69`  
		Last Modified: Wed, 10 Nov 2021 03:48:06 GMT  
		Size: 4.9 MB (4924623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
