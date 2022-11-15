## `redmine:5-bullseye`

```console
$ docker pull redmine@sha256:52d68bc62e6ef34499e3204237905bd887768d57658cce8e7b500414b178b16e
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
$ docker pull redmine@sha256:26ed292e30ef92b7200192d01ba964b88266f36ac288f75bc63bd55668106428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.0 MB (237041138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cc28c5d18648ded35d26ca41838853157f53003dd000ca90e6803d2bcb3f9a4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 09:02:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:02:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 09:02:08 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 09:07:54 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 09:07:55 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 09:07:55 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 09:10:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 09:10:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 09:10:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 09:10:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 09:10:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 09:10:20 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 09:26:40 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 09:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:27:12 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 09:27:13 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 09:27:13 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 09:27:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 09:27:13 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 09:27:13 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 09:27:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 09:27:17 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 09:27:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 09:27:50 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 09:27:50 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 09:27:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 09:27:50 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 09:27:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cc1987b4c3d3fdb89192cea3fd492e595844522888b2bdfb7bc0e15d9c38f`  
		Last Modified: Tue, 15 Nov 2022 09:24:02 GMT  
		Size: 10.0 MB (10020448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e7129cddea3dc930d634f547f58a869e692c5ea4b3183760620cfc8ec67fb7`  
		Last Modified: Tue, 15 Nov 2022 09:24:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ebe3be8da43ad18f7bb4ed7711959328c6c9bc23c874d0f827fe9afc3b5e24`  
		Last Modified: Tue, 15 Nov 2022 09:24:38 GMT  
		Size: 32.4 MB (32436969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea2535835d7dbc570141035d49ce6acfad3726f456824892ea3fb88fc120278`  
		Last Modified: Tue, 15 Nov 2022 09:24:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66b686a2992c4925e7a214caeab3300e321b7a09dc6ae8f5c4840aa9379e3bd`  
		Last Modified: Tue, 15 Nov 2022 09:30:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be4d09540aa8d0a9709718e827e5b254414d99d4d1d5ec23d520071944f9ee6`  
		Last Modified: Tue, 15 Nov 2022 09:30:39 GMT  
		Size: 102.0 MB (102023896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876658288fc3cbcec7a0d4ee83eb0ccfec7a5be4afbc7b0e1990543b9b68fd41`  
		Last Modified: Tue, 15 Nov 2022 09:30:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429dd14d23bbf669ba4ae905c749ce390f376bd34e2f04e1e571929821478c89`  
		Last Modified: Tue, 15 Nov 2022 09:30:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcfc56ee84785dc51b19b64f19555ce2f1eab5bc9437f5a435841b620afb6a9`  
		Last Modified: Tue, 15 Nov 2022 09:30:23 GMT  
		Size: 3.1 MB (3141779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ea11528bbcafd483bb16e42d4a59458112c46d1cc735aed8a75c6f9624743d`  
		Last Modified: Tue, 15 Nov 2022 09:30:28 GMT  
		Size: 58.0 MB (58000968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decc661f1394554726b9dce061be0a226caaea62e561403dd8328ec75978acab`  
		Last Modified: Tue, 15 Nov 2022 09:30:22 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:dc6f86d5f9f1fde79c0688f6841ca8ed64be0a994ce783bc6e8fcaabf56fc6dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235966189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2c4c54c27cc8f13aac2acdce2bf10572e3b59488f6a1c5a4bb59ea06e8781d3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:54:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:54:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 04:54:15 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 04:57:13 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 04:57:13 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 04:57:14 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 04:59:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 04:59:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 04:59:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 04:59:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 04:59:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 04:59:51 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 13:46:18 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 13:46:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:46:54 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 13:46:54 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 13:46:55 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 13:46:56 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 13:46:56 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 13:46:56 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 13:46:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 13:47:01 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 13:49:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 13:49:08 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 13:49:08 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 13:49:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 13:49:08 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 13:49:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450954c5c7cc28fe73779bdbd643e8b1ec357322152ee95a529cc670f305bee`  
		Last Modified: Tue, 15 Nov 2022 05:07:29 GMT  
		Size: 8.6 MB (8634285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9429e4a2b25420ad119749abb1d398ea170da0694490727f3873fce80f791c08`  
		Last Modified: Tue, 15 Nov 2022 05:07:27 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87e40a1a628ccb8f753c8327eefc51e44939de5bc2d887f58afa121c53abe3f`  
		Last Modified: Tue, 15 Nov 2022 05:07:59 GMT  
		Size: 31.0 MB (30985914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349385e7cfb4b0df50f7a2cef0c9c2246b5b8a90c730b187fb288e6e2b8cd8a4`  
		Last Modified: Tue, 15 Nov 2022 05:07:54 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f409b9f9d9ddf861bfbd1c8f0de2c545d97aed76bfe315f659bfe827a68a0c3`  
		Last Modified: Tue, 15 Nov 2022 13:53:13 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f055fc018b06fef8709d4f38dda5a9b60b3a2673e14047ea8a5555662e284d72`  
		Last Modified: Tue, 15 Nov 2022 13:53:32 GMT  
		Size: 97.0 MB (96988095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb1559b74dd8cb173f39f1204aa8fe47f3cc2e5c1c060d3a67f7e017126053`  
		Last Modified: Tue, 15 Nov 2022 13:53:11 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da0550c6f89f4c77acb23f35222771cc4589c6d1aeededdfb7a040bf569ab48`  
		Last Modified: Tue, 15 Nov 2022 13:53:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd2be8082371b82768a24929b234ec4aab7e72473f9524735622f3f99cc15e5`  
		Last Modified: Tue, 15 Nov 2022 13:53:12 GMT  
		Size: 3.1 MB (3141313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c74e2cf5c52cf106db4a535b93d08f2dd5de92bbf049768f5ae44e10540060`  
		Last Modified: Tue, 15 Nov 2022 13:53:21 GMT  
		Size: 67.3 MB (67298113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eff3140802bb3a16859dcfecb4f511c406ce5338e40d2c91fe3b90d796e76c1`  
		Last Modified: Tue, 15 Nov 2022 13:53:11 GMT  
		Size: 2.0 KB (2010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:746c1ea9b843a16e7f4f9a4b12fb88d607c01b91f39958f6375a40e003465a83
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228860696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f398b2bdc467ac2b64cfe1da71fea3725561966256c6d69264529f3b1ec1932`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:40:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 10:40:58 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 10:46:44 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 10:46:44 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 10:46:44 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 10:49:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 10:49:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 10:49:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 10:49:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 10:49:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 10:49:06 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 11:10:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 11:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:11:32 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 11:11:32 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 11:11:32 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 11:11:33 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 11:11:33 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 11:11:33 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 11:11:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 11:11:36 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 11:13:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 11:13:29 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 11:13:29 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 11:13:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 11:13:30 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 11:13:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f882748051d83dfb7f7453eeae956b960128447af5d1008295343c9993eb850`  
		Last Modified: Tue, 15 Nov 2022 11:07:13 GMT  
		Size: 8.1 MB (8142757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b303dec2f3fb882d25d0bd1ba1514dae7537c52955b36b8e35ab34bec8868a`  
		Last Modified: Tue, 15 Nov 2022 11:07:11 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403f56f4d1c68bc8b46225b8dadf17f2c61351bd4c0073fabee3d8f879dd043d`  
		Last Modified: Tue, 15 Nov 2022 11:08:02 GMT  
		Size: 30.8 MB (30848936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41a84ea6c480831479df4c6b67b2958abfcaf4405c82223ceeb09345d4ac2d4`  
		Last Modified: Tue, 15 Nov 2022 11:07:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250dfd5c2481c0e66e9967142b7efa8222aa65e2f6ff2c7cc407c9021a140bd1`  
		Last Modified: Tue, 15 Nov 2022 11:17:53 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f970287dd4b04fb728f2b39d2afa470d2aa0a38b9e28b37825d5ae36127932`  
		Last Modified: Tue, 15 Nov 2022 11:18:10 GMT  
		Size: 93.1 MB (93134583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516ac86668cd8342fc3b97a102cbc2fe8ac2a99f97f41a1accca52014a352e79`  
		Last Modified: Tue, 15 Nov 2022 11:17:51 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abe7867462e037a5c96c96ab126e60c4cb854c4f4bcde7eaa640bf762b50ace`  
		Last Modified: Tue, 15 Nov 2022 11:17:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223b6f2c1d20e1fdd7bdf74572bf421610bc7aed72d31cbf187f27748c9ff1c`  
		Last Modified: Tue, 15 Nov 2022 11:17:52 GMT  
		Size: 3.1 MB (3141305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598bd9f613d388155485d62edb94b2032bbd1a002c128a0201e010c05b3f5882`  
		Last Modified: Tue, 15 Nov 2022 11:18:01 GMT  
		Size: 67.0 MB (67012574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d584e5496acd4e70590221c7206f27751f4cbc90a134c7d37ae384f4550e70`  
		Last Modified: Tue, 15 Nov 2022 11:17:51 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:bd5e11ed08983589491695c683e12c12748415938ae7a5ef357ecb2fdc85a727
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231517137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43fe07ae3a7ee8a0b932e84ec7086a9697314392829178c89d4587af68f36dee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:26:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 04:26:30 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 04:35:50 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 04:35:50 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 04:35:50 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 04:37:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 04:37:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 04:37:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 04:37:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 04:37:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 04:37:32 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 18:17:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 18:17:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:17:47 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 18:17:47 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 18:17:47 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 18:17:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 18:17:47 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 18:17:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 18:17:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 18:17:50 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 18:18:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 18:18:19 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 18:18:19 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 18:18:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:18:19 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 18:18:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85093415d82731b157cf4fc91571afad739e980b93e7e69b9d9876bf0daed48`  
		Last Modified: Tue, 15 Nov 2022 04:48:01 GMT  
		Size: 9.2 MB (9242687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e465289e24c0bcf6f03c8171c71f4f378c6decdd1fc3b9c03be11e15afefcc12`  
		Last Modified: Tue, 15 Nov 2022 04:47:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820a1bb95a80133b22386b22078153b2fff48197ff4a25b818678f67f74077c6`  
		Last Modified: Tue, 15 Nov 2022 04:49:03 GMT  
		Size: 31.8 MB (31805884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfcd5d8a4f4d5b3f0998d56463b9408d0086b0377da2ff787cc9f3fb43a4d8d`  
		Last Modified: Tue, 15 Nov 2022 04:49:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5bea0193b1b61695be18ededce44d0fc992522d8e64d8317b92a1d842821fe`  
		Last Modified: Tue, 15 Nov 2022 18:20:14 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d71b2eed04effdf5c97f4ecd2c640dced9d0e63fc0b150457d945be2b61f478`  
		Last Modified: Tue, 15 Nov 2022 18:20:26 GMT  
		Size: 99.8 MB (99800140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2994d30f0afd29ddae6cd0453ad8e3f755a7403573c30fbb687865a3489eb5a`  
		Last Modified: Tue, 15 Nov 2022 18:20:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bf7d009a6291172f4b352368ef99f7325c3c2c95feaac7c15f1866cd411dec`  
		Last Modified: Tue, 15 Nov 2022 18:20:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a2dc8693288bef7fe01199714793d9fc0bf8bb90ee02f698e723f349ba03e4`  
		Last Modified: Tue, 15 Nov 2022 18:20:13 GMT  
		Size: 3.1 MB (3141783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7d878c01b264ef17a54fd9c6d50406f167e1ebc976b48c0dc58cbe06d269c4`  
		Last Modified: Tue, 15 Nov 2022 18:20:18 GMT  
		Size: 57.5 MB (57461587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c2007adf5ce2c612fb639722b8044339e948af5afbd280e74ed169a16aabf`  
		Last Modified: Tue, 15 Nov 2022 18:20:13 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; 386

```console
$ docker pull redmine@sha256:65fea5c68c5d75fa05ef8b8ef0d7d50c4510b61f9bb2428bc0f8b0d864f31590
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238647869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e21e23f6a4d433ccba3c1288e7a2b9ed58465b7e9d8c5baf55c81a4fd8f471c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:57:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:57:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 05:57:44 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 06:10:58 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 06:10:59 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 06:11:00 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 06:13:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 06:13:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 06:13:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 06:13:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 06:13:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 06:13:18 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 20:58:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 20:59:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 20:59:27 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 20:59:28 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 20:59:28 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 20:59:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 20:59:30 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 20:59:31 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 20:59:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 20:59:36 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 21:00:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 21:00:10 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 21:00:11 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 21:00:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 21:00:12 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 21:00:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257717017759bee815eb41bf0d6827ac66d5118fe308714222dc7c2be841de9`  
		Last Modified: Tue, 15 Nov 2022 06:29:09 GMT  
		Size: 11.8 MB (11788329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e786a9905383f130024a7e5cb2a41a9d508bd8482d83be57037287b279229b0`  
		Last Modified: Tue, 15 Nov 2022 06:29:07 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be05dbc9d410295913e9455654e15a925113a79e93153d211198738f9e9a6d84`  
		Last Modified: Tue, 15 Nov 2022 06:30:28 GMT  
		Size: 30.8 MB (30789359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195f640db1ba195e06c927ccdef5f4a4be8f5f6e4de276d5007ec95c3d8d2a8`  
		Last Modified: Tue, 15 Nov 2022 06:30:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedd37dd6bd8e8c2db03a7c1e68377a7e1585297b82475cb31526558dbd8cb25`  
		Last Modified: Tue, 15 Nov 2022 21:03:16 GMT  
		Size: 1.6 KB (1611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f8c56c2e7793bb80040c637ade32eaaf34c4d1199528aeb2a0576ddbeefb72`  
		Last Modified: Tue, 15 Nov 2022 21:03:32 GMT  
		Size: 103.4 MB (103354884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8b1d95038d88687074a536171a285a2ff99b851a7bcad8be131fdc1b09e4ce`  
		Last Modified: Tue, 15 Nov 2022 21:03:14 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcdf627f210c227037843ed440567aca926573f9639fed62199ab637fb4c1b1`  
		Last Modified: Tue, 15 Nov 2022 21:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dee14521ecf4c7c1d8885921d7e3986e3db3acd44be06d6608669ec7f55bb9`  
		Last Modified: Tue, 15 Nov 2022 21:03:15 GMT  
		Size: 3.1 MB (3141543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7b7783bb9313a91899c9388491a1cf083ae616c6ee1d337cd6ed3870f7d0f8`  
		Last Modified: Tue, 15 Nov 2022 21:03:23 GMT  
		Size: 57.2 MB (57176543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250e6f8e4a843cdf423d9277259c35193607c4e3a824ddb4ffaa82d1f306aedb`  
		Last Modified: Tue, 15 Nov 2022 21:03:14 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:c66ec1560af93112cd9e2db7aafb2441a1c2836f0a8a0f10c197a25f983c7349
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259082300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a6fd4b5b7072c33a67e885f161ff6d19f500068f3990a04e2193a6c7236792`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:19:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:19:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 10:19:06 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 10:24:15 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 10:24:16 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 10:24:16 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 10:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 10:28:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 10:28:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 10:28:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 10:28:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 10:28:25 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 10:41:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 10:43:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:43:06 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 10:43:06 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 10:43:07 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 10:43:08 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 10:43:08 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 10:43:08 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 10:43:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 10:43:14 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 10:46:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 10:46:26 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 10:46:27 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 10:46:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:46:27 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 10:46:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dfdc42736e7b5d86d42ae43d2d3d33bc51229341c90465b349f23bff5995b0`  
		Last Modified: Tue, 15 Nov 2022 10:39:26 GMT  
		Size: 10.5 MB (10478766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b7377b9eeeaf50b9e7c6d3d2d0ff8b424dd9b359398fdddb5109d0166a4f36`  
		Last Modified: Tue, 15 Nov 2022 10:39:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cd0a799bcbafa9836c5e62603df4d384e3844d4074b59953c8d5d61ab47f41`  
		Last Modified: Tue, 15 Nov 2022 10:40:00 GMT  
		Size: 32.6 MB (32601421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d973a09caa88914eede9d04488761e13555f8b3bb3fde9b4297945382f1fc40e`  
		Last Modified: Tue, 15 Nov 2022 10:39:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e7f8ce3cfe6202cb1821e26a11a48d29c3c95e52b31443d7f8e6a969e12d99`  
		Last Modified: Tue, 15 Nov 2022 10:52:58 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8982c4cab89d042b4e631c5075bc60a7808049d28f8403bf3361970a8e8d553`  
		Last Modified: Tue, 15 Nov 2022 10:53:26 GMT  
		Size: 107.5 MB (107520078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9aeb8e3c4378f8420e0d703bb8f21d50b3640551361131d60666c8994e33cd0`  
		Last Modified: Tue, 15 Nov 2022 10:52:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61dde01a3ae394e87fb681cb4e7077b009d40ffa9227652e12ff5ecb0301436`  
		Last Modified: Tue, 15 Nov 2022 10:52:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c38153f00f8ae6f3d7c1a226b897b46d6d70de6864d5fe439408d38055d45`  
		Last Modified: Tue, 15 Nov 2022 10:52:58 GMT  
		Size: 3.1 MB (3141781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9624098257750d90f2cd83d75664bc0882412d447a62b557bb0516e854f32a8`  
		Last Modified: Tue, 15 Nov 2022 10:53:09 GMT  
		Size: 70.1 MB (70050660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa559862e29369dde537ebbe342f4e11e9b86a499e87da1c808d90645555eea`  
		Last Modified: Tue, 15 Nov 2022 10:52:56 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:1df40285b62d2f1916a00f350bc4da30e9bb622d0db3a9de80384a52db269c39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.7 MB (242716157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce6fe36735559c33590ba8e30ecc9a3ec84174832df142bb83f1574fcdafaea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:21:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:21:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 15 Nov 2022 05:21:10 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 05:30:28 GMT
ENV RUBY_MAJOR=3.1
# Tue, 15 Nov 2022 05:30:28 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 15 Nov 2022 05:30:28 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 15 Nov 2022 05:33:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 15 Nov 2022 05:33:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 15 Nov 2022 05:33:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 15 Nov 2022 05:33:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 05:33:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 15 Nov 2022 05:33:32 GMT
CMD ["irb"]
# Tue, 15 Nov 2022 18:28:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 15 Nov 2022 18:29:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 18:29:37 GMT
ENV RAILS_ENV=production
# Tue, 15 Nov 2022 18:29:38 GMT
WORKDIR /usr/src/redmine
# Tue, 15 Nov 2022 18:29:38 GMT
ENV HOME=/home/redmine
# Tue, 15 Nov 2022 18:29:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 15 Nov 2022 18:29:41 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 15 Nov 2022 18:29:41 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 15 Nov 2022 18:29:42 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 15 Nov 2022 18:29:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 15 Nov 2022 18:32:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 18:32:08 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 15 Nov 2022 18:32:09 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 15 Nov 2022 18:32:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 18:32:10 GMT
EXPOSE 3000
# Tue, 15 Nov 2022 18:32:10 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff38e36c409c10fb8e82e79fe8bd09d3c2dfb473a7adf4fbaf95ab9b050a1460`  
		Last Modified: Tue, 15 Nov 2022 05:42:49 GMT  
		Size: 8.9 MB (8860439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d618cd95d9b3b0de81d0f4defafddc43a54a0536989430dd84c4b2209797d0`  
		Last Modified: Tue, 15 Nov 2022 05:42:47 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd190d800555ad4adc56f056f98736be1f7a4973d39ea54015842bff711561a3`  
		Last Modified: Tue, 15 Nov 2022 05:43:37 GMT  
		Size: 32.3 MB (32250033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a215531acccf591a8018ca78fdb489a7405a4f01d7641a79b5616b63d3ad1edb`  
		Last Modified: Tue, 15 Nov 2022 05:43:34 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdf997c09f059cc6288062524b6dcf9fe72c0eea6490dcf0c8dacae9ff9840e`  
		Last Modified: Tue, 15 Nov 2022 18:37:20 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7acc8a81568cf1753549a66ee055f852ac6d75807bcfa5daf5f0f8c9638afc`  
		Last Modified: Tue, 15 Nov 2022 18:37:33 GMT  
		Size: 99.2 MB (99156305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c85baf8e140cf4135494e6307561e0bebec8599458cdb4a7d52e4b008f9357d`  
		Last Modified: Tue, 15 Nov 2022 18:37:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9a68a0573881dd62a35f7384e9f9da20a6b09b225562236e14fa91ca2f05e0`  
		Last Modified: Tue, 15 Nov 2022 18:37:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd4bf3a403457bf8bb1980aa4f78e578dade4095e136a4cb757049ae577a52c`  
		Last Modified: Tue, 15 Nov 2022 18:37:19 GMT  
		Size: 3.1 MB (3141784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590e99f710498bdbf95e3d895dc2c1f5febdd3075bf531f0f1f9ff3ef0e7cde1`  
		Last Modified: Tue, 15 Nov 2022 18:37:25 GMT  
		Size: 69.7 MB (69659359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e588907cd2eab8f44fcd420108922fedb29a517fb39f7507a2c20dbd25192f28`  
		Last Modified: Tue, 15 Nov 2022 18:37:18 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
