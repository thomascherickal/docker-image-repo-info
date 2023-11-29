## `redmine:5-bookworm`

```console
$ docker pull redmine@sha256:28979464f14ec53f447617a037f43975a08612d94dd7de09fdc2a9d35185f45c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redmine:5-bookworm` - linux; amd64

```console
$ docker pull redmine@sha256:b56e3e227f1f221ba79623d512c9560373a04bfc8d36e9f84a4aa7d539c22d4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269638188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402ee5eeeaaa7d5aaff2c9203683b835c9b242e893c98b90ca8d117a507c249e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:23:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:23:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 09:23:40 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 09:35:39 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 09:35:39 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 09:35:39 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 09:38:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 09:38:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 09:38:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 09:38:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 09:38:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 09:38:05 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:032f78a9a8d56c57bc1daf27956c8bac0c9a0bdb7d7934d0068a10982453a304`  
		Last Modified: Tue, 21 Nov 2023 09:46:37 GMT  
		Size: 13.9 MB (13853569 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49e36bd6cba5164fde3c6284b9dddded584fe2a620d97d5b24e73828ad634939`  
		Last Modified: Tue, 21 Nov 2023 09:46:34 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6abe30ec3479e1965e12fbe6b80ab66e1936617161f29edf6b51b1334f1178c9`  
		Last Modified: Tue, 21 Nov 2023 09:47:56 GMT  
		Size: 32.9 MB (32924006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e87ef05cb8dc72e1d6ac40fd7c04febb3d3542b45f9d0ea33363189b56f25888`  
		Last Modified: Tue, 21 Nov 2023 09:47:54 GMT  
		Size: 177.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f119cfdb2fe199f4cea40ad1f54ef1b5a2b056a66f22621f7cd07f8e028b1628`  
		Last Modified: Wed, 29 Nov 2023 17:34:40 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89fb2e492280ec8349f02ba2933ed54458a2db371ab43bd2cbaa2693d7376246`  
		Last Modified: Wed, 29 Nov 2023 17:34:42 GMT  
		Size: 123.1 MB (123111660 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54e1525498ff94edb927696c6b4a10100fd148b86c106e0e2c469366cdd25ad3`  
		Last Modified: Wed, 29 Nov 2023 17:34:41 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:223755aae0ede36f3015fcb08df01eed75ef222f25b4d02906f9f10761f4d25e`  
		Last Modified: Wed, 29 Nov 2023 17:34:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89d86f1a9e88453334b6624f306f8039f1dddd22ce4a7299cc0639075dd04866`  
		Last Modified: Wed, 29 Nov 2023 17:34:41 GMT  
		Size: 3.2 MB (3235219 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d9f5e417573c7b901ebc249c2b6bb50eb5230bff2befe02001e8d76b4dcd9a8`  
		Last Modified: Wed, 29 Nov 2023 17:34:42 GMT  
		Size: 67.4 MB (67360062 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f652466407805912fba0c62ea95619c3c6ef217a50f937844d09c0b0ebd6c7d2`  
		Last Modified: Wed, 29 Nov 2023 17:34:42 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:b09b164760b0fb172392abbedf64d8d4ecccee432b7c2df15a47a3ddb1dd4669
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7589544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919131e878450de00d1865d0ec84f4a61c54d0d5d122c9d951bb599116f21ffd`

```dockerfile
```

-	Layers:
	-	`sha256:b9e6212a97a41065a7714415001b2a2f08c6147847f8f59dc78dea8b5d616533`  
		Last Modified: Wed, 29 Nov 2023 17:34:41 GMT  
		Size: 7.6 MB (7553795 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6a65a26f9a3d6e93446042f4320fcac7174157db3d9c0fdbc0edd378914b11c4`  
		Last Modified: Wed, 29 Nov 2023 17:34:40 GMT  
		Size: 35.7 KB (35749 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; arm variant v5

```console
$ docker pull redmine@sha256:a0307c90178cbcaaefbc976852f16860dc8a09d0accd0c0c5c917a885de374b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254081948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7595316f40a1a92c10c8254a299f949075b74eb65efec1288b76dd1a6f95b07f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:24:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:24:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 05:24:17 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:35:42 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 05:35:42 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 05:35:42 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 05:38:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 05:38:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 05:38:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 05:38:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 05:38:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 05:38:20 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1419f74c8ddf1a69b166650147f00ab01d5978c69f29e5d697a51548cf202bcd`  
		Last Modified: Tue, 21 Nov 2023 05:44:12 GMT  
		Size: 11.6 MB (11611274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:489d0dec931ffd61d84c5c26f294fe5f5f81cd7062000041db62cacbc9f5d85e`  
		Last Modified: Tue, 21 Nov 2023 05:44:09 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f172f89e2739bc6c5743aed1bb63db4559b51217e7f3e4855d78a4743972170`  
		Last Modified: Tue, 21 Nov 2023 05:45:26 GMT  
		Size: 31.7 MB (31717676 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3940d2c43c6f89f01f890e7c8b7b336ab69dcfe35a54405c9c3a6884a762df81`  
		Last Modified: Tue, 21 Nov 2023 05:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7cc5b6c77393fd10ad0292f3e9326748f48619715cc5ab6987185360439b9c0`  
		Last Modified: Wed, 22 Nov 2023 03:56:12 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f7accfd60e2a0181ab6385313a959afaa65403f94e11e9c5e7c0ca00d9e2f21`  
		Last Modified: Wed, 22 Nov 2023 03:56:15 GMT  
		Size: 116.6 MB (116634196 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94de6854d5d5f65d174fa3b973abc25c1f4314fa82c42a2f1547104fb8c2c090`  
		Last Modified: Wed, 22 Nov 2023 03:56:12 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:235fba6cbff154b8fd3887f48fe514b09bdb573f669fc637aa703bfb3ada1ec3`  
		Last Modified: Wed, 22 Nov 2023 03:56:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70eee9f579dc104ca388c216aba3bb1ba0adccf709af0095c111f5bb39dbabc9`  
		Last Modified: Wed, 29 Nov 2023 08:00:09 GMT  
		Size: 3.2 MB (3235223 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01759437f8526232a4b40010ae0600fd3b2e0be4565bba30d6355183bae6fbaa`  
		Last Modified: Wed, 29 Nov 2023 08:00:10 GMT  
		Size: 64.0 MB (63957667 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0de0b119a8dc3bac332fbc31de253f118417a38aaf8e798570531ac5924a17b5`  
		Last Modified: Wed, 29 Nov 2023 08:00:08 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:f0f617fde70edbeec01bafc2ee2975e72563ac9e86140feae0d0aa3531ff1b52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 KB (34873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f37fed96e0aad1818ecd6dde8baedd20af8ff35407f0083d01c9980bba1966`

```dockerfile
```

-	Layers:
	-	`sha256:7233e72927c3cdb0da7e4ad3dac845f015094d6a474b1059831f72e93a21c848`  
		Last Modified: Wed, 29 Nov 2023 08:00:07 GMT  
		Size: 34.9 KB (34873 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; arm variant v7

```console
$ docker pull redmine@sha256:41fce200c5d4586ff552eb95a791fd7e3514bd25ca47f85e678ad71c9dc29c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246325919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1475827ffb919dc1ad938f30fef98f761c15c8dbce59034dfd06ea398dc557`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:48:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 07:48:09 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 07:58:43 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 07:58:43 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 07:58:44 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 08:01:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 08:01:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 08:01:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 08:01:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 08:01:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 08:01:06 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9eb59b5ea2ceca98e0bcbe78eb7c42871527ba40c15098e8eaabc421711654f`  
		Last Modified: Tue, 21 Nov 2023 08:09:06 GMT  
		Size: 10.9 MB (10947526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32aa949edac2235060c6b922f7e6a25a02706f12917ef161723b979775298104`  
		Last Modified: Tue, 21 Nov 2023 08:09:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d17800a4b05bb4c000e0ff43b71205422bec2a80ed158bc51c4abd4070f71d36`  
		Last Modified: Tue, 21 Nov 2023 08:10:28 GMT  
		Size: 31.6 MB (31560864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14cb830a65b96764e6ffb25dda0d8333a596deecc2e37870e42b87cd7492f372`  
		Last Modified: Tue, 21 Nov 2023 08:10:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d9cb93ac4fea0cdb300941f75bfd50f438b02dcfa2af65afe88efe1b90db2bc`  
		Last Modified: Wed, 22 Nov 2023 04:34:42 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:162994d2beda1cd4093c29c340aa1a6d16b04f1a3d0f2e3126a900915d9c082d`  
		Last Modified: Wed, 22 Nov 2023 04:34:46 GMT  
		Size: 112.1 MB (112146836 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:452909102d366e6dc5f55e0bb967e7767c92e6a0532a29624b2940eaac6a80bd`  
		Last Modified: Wed, 22 Nov 2023 04:34:43 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:448136f5a6b35e56c6ed4a5ac87cf88b200d5c9fa64a6173aa7cc44a2b8f2602`  
		Last Modified: Wed, 22 Nov 2023 04:34:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a75a727d3e280c46f9e1b9d9d2551cfd018440c66e06b0935590387743cd4601`  
		Last Modified: Wed, 29 Nov 2023 10:41:07 GMT  
		Size: 3.2 MB (3235217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c08dafa8e836bc387e103bde4cc536e484a4b910f31dd3df719f822a305214b2`  
		Last Modified: Wed, 29 Nov 2023 10:41:09 GMT  
		Size: 63.7 MB (63682793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1114c6a1b99f075eca277cc09a2438d2c1bbf0769b10528058fc26457e448b7`  
		Last Modified: Wed, 29 Nov 2023 10:41:07 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:96907adc38f3e643ff8fa052c184e66ccfe1d1c15a2c3717a5d42dce9eb9d684
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7559183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962eea20aa535fca11029457884b9fd63b45c36ede7162ec39ecd5b35e82cb40`

```dockerfile
```

-	Layers:
	-	`sha256:305f340db4bd4f638d79836dfa53ee60c4d5bb09298012680113582d25febf06`  
		Last Modified: Wed, 29 Nov 2023 10:41:07 GMT  
		Size: 7.5 MB (7524095 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:75717a5ce34df18c39cc4e5373ff686037e91c7cd7557fe4427c7e931dd679c3`  
		Last Modified: Wed, 29 Nov 2023 10:41:07 GMT  
		Size: 35.1 KB (35088 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:02bd7c1b265001bf05209395a002c4703208d4975039662a00a2b8578c84e533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.5 MB (264457790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19637d60a5b24a19260153705263bbff894e78a99edee444ae7a898973f73531`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 19:53:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 19:53:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 19:53:37 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 20:10:37 GMT
ENV RUBY_MAJOR=3.1
# Tue, 21 Nov 2023 20:10:37 GMT
ENV RUBY_VERSION=3.1.4
# Tue, 21 Nov 2023 20:10:37 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Tue, 21 Nov 2023 20:12:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Nov 2023 20:12:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Nov 2023 20:12:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Nov 2023 20:12:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Nov 2023 20:12:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 21 Nov 2023 20:12:30 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:577cd8c89ac1e6f3d263821a0f543fc92600e3853758016adc611e56658c87ec`  
		Last Modified: Tue, 21 Nov 2023 20:24:21 GMT  
		Size: 12.7 MB (12695296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4129eaee70b6fafd86d065814443b63cb073f297ff7d8d13d8487dcdfdd748a1`  
		Last Modified: Tue, 21 Nov 2023 20:24:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0580a048f2c6f1a820184073d759883c86a118ac850cc2990da8c9f961502365`  
		Last Modified: Tue, 21 Nov 2023 20:26:38 GMT  
		Size: 32.4 MB (32361792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:443a2ac35cf390896d7179987ab10ab056b625bb658ca71eb546c04b8dc7ce62`  
		Last Modified: Tue, 21 Nov 2023 20:26:36 GMT  
		Size: 177.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc0bd427a53d0da576a43226058fbee62aaff40416592d4a1b95e97bd4495b25`  
		Last Modified: Wed, 22 Nov 2023 12:28:48 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c9d1ae14f1a65b516af9dfd6aeff2d0b06ebf11b3361ed643240367dd633336`  
		Last Modified: Wed, 22 Nov 2023 12:28:51 GMT  
		Size: 120.2 MB (120239733 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12572b6fbc66a8a165bc3c64b0b5e915bf835d535f8d5e2cb0344be3f2493c55`  
		Last Modified: Wed, 22 Nov 2023 12:28:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2798a917b1eef368f04545c169ed5be127cb16b4f1d8fd1617c75d34b240327`  
		Last Modified: Wed, 22 Nov 2023 12:28:49 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:435c0a1b29da697bca6dd460b7049a8808fd024e086e548b2208f04058daaae8`  
		Last Modified: Wed, 29 Nov 2023 06:11:00 GMT  
		Size: 3.2 MB (3235229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d080a8a69a7c763ed0c7d5e92b9437f46a597f96be7ccd15c1f573eb6087122b`  
		Last Modified: Wed, 29 Nov 2023 06:11:01 GMT  
		Size: 66.7 MB (66742704 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:052a5afbbcfde47359f59c92a8145df769fac149022aab5162a584c26ebc2d2f`  
		Last Modified: Wed, 29 Nov 2023 06:10:59 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:a6c269697d8ddb9fdb3bee2361af1f16f2b35c5a2a5d7e729b02aaa7e532fccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f78b9f18cac52428687b00e0a6749563fa776e5d9c62b1a2b79f71a1f55df74a`

```dockerfile
```

-	Layers:
	-	`sha256:8c85930588842346c285ff3c14f5eddf00c7add7b18110daa6e710cc3ee11098`  
		Last Modified: Wed, 29 Nov 2023 06:11:00 GMT  
		Size: 7.5 MB (7534711 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:019199157280c0ca0f1318dd32d576277d8430f9e75168d72b1d8478bc50595e`  
		Last Modified: Wed, 29 Nov 2023 06:10:58 GMT  
		Size: 35.0 KB (34952 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; 386

```console
$ docker pull redmine@sha256:b850450c0d11d93e191d2dab0071aacf317d778712e8835a0b57bc65e3f09603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264819095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dbcfaff76ea1ce27eae903370ddca21397aff208a9cc3082ae791fced662ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 30 Sep 2023 08:26:15 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["bash"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 30 Sep 2023 08:26:15 GMT
ENV LANG=C.UTF-8
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_MAJOR=3.1
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 30 Sep 2023 08:26:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Sep 2023 08:26:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["irb"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RAILS_ENV=production
# Sat, 30 Sep 2023 08:26:15 GMT
WORKDIR /usr/src/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
ENV HOME=/home/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_VERSION=5.0.6
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.6.tar.gz
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=488fe08f37a8eb1011415922a8ea743b7f38d8a7a5f8822950a34a375dcf08ee
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 30 Sep 2023 08:26:15 GMT
COPY docker-entrypoint.sh / # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 08:26:15 GMT
EXPOSE map[3000/tcp:{}]
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26f9abe942e705f9fe869e919260dea8dc7015ace1c892fb673cd3da4bde734e`  
		Last Modified: Wed, 01 Nov 2023 07:56:54 GMT  
		Size: 13.4 MB (13402315 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b3d589a42085e031e339dc67c22c9f1e541916d649cfc826bc99e1886bfbb4`  
		Last Modified: Wed, 01 Nov 2023 07:56:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05c83b44c78d8ea4fed78da37fdbbe17ff6f91869c5d8e19056692c4921d35b1`  
		Last Modified: Wed, 01 Nov 2023 07:58:17 GMT  
		Size: 31.6 MB (31626535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae54c90a4f4c2ac69cd7d2721345c1b2bf6a350c21f9a3287694f21b8b8fcd46`  
		Last Modified: Wed, 01 Nov 2023 07:58:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a817347238bf30660f09e0488a00f385c37ed1c0a0fec604216dd56877b8f1a2`  
		Last Modified: Wed, 01 Nov 2023 10:56:40 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3045896023de6fbaf6bee837e77b0da3540368cea5f36e3126adf1b1b15705`  
		Last Modified: Wed, 01 Nov 2023 10:56:45 GMT  
		Size: 124.9 MB (124941270 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bfc0cf001486f29d3c7429b5cf3937d09855d26225d20be9b801702b72a2808`  
		Last Modified: Wed, 01 Nov 2023 10:56:41 GMT  
		Size: 138.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7bc166b634a1d91942839b40ea46f5441bc62736f22ccbe688b3f27714850e1c`  
		Last Modified: Wed, 01 Nov 2023 10:56:41 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3fb0e631e10afd0753394243089ae43298169d240c88c83da4358187c11419f`  
		Last Modified: Wed, 01 Nov 2023 10:56:42 GMT  
		Size: 3.1 MB (3146238 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f40cddca8fc9bf8252931b4b0bf37597a36f37c99d88adb4c9b92bd7ae6a653`  
		Last Modified: Wed, 01 Nov 2023 10:56:45 GMT  
		Size: 61.5 MB (61534937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b6f238505a8be913f0b66be06706a2d4773b24947bccc2a617213176c15e34d`  
		Last Modified: Wed, 01 Nov 2023 10:56:42 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:d0d0975eeac5780d1736358a20939840d1cd5a70231981c00a771c9ac083db7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 KB (35296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042d9b7b5af9316a027e2968401599de3bc583ed77a18eb4638cc431f6a88793`

```dockerfile
```

-	Layers:
	-	`sha256:e6c98c4664085bc01863e4ea72e88961cafaed727a8c43ef2f1a945d4aea9106`  
		Last Modified: Wed, 01 Nov 2023 10:56:39 GMT  
		Size: 35.3 KB (35296 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; ppc64le

```console
$ docker pull redmine@sha256:763d4565b9ef5646955fbdd42ce773798961ee36aed42c7d11084ca2d4a5b095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290053970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be266977e0de1458bb4a15875a2816d743b4c3313b35751a86363f02fe259ba3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 30 Sep 2023 08:26:15 GMT
ADD file:f36d600ab8508979b5763875a75f35555fa0a83d2656cbcdfa50978c6ae97353 in / 
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["bash"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 30 Sep 2023 08:26:15 GMT
ENV LANG=C.UTF-8
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_MAJOR=3.1
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 30 Sep 2023 08:26:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Sep 2023 08:26:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["irb"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RAILS_ENV=production
# Sat, 30 Sep 2023 08:26:15 GMT
WORKDIR /usr/src/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
ENV HOME=/home/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_VERSION=5.0.6
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.6.tar.gz
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=488fe08f37a8eb1011415922a8ea743b7f38d8a7a5f8822950a34a375dcf08ee
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 30 Sep 2023 08:26:15 GMT
COPY docker-entrypoint.sh / # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 08:26:15 GMT
EXPOSE map[3000/tcp:{}]
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e56c8f20d7d119ff87eb044f21bfd5a4b30bf8436fc5fac12871095a6bd1517c`  
		Last Modified: Wed, 01 Nov 2023 00:26:10 GMT  
		Size: 33.1 MB (33141482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc8ac2acec68c8f8c0c6901d20ead919a0d653e02a21a254c1b9dc6e1ac68863`  
		Last Modified: Wed, 01 Nov 2023 11:34:24 GMT  
		Size: 14.6 MB (14574643 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d97698c92f91a59342a5f2fad255a0cbafe6323344d3331fda5e69e3aed986b8`  
		Last Modified: Wed, 01 Nov 2023 11:34:21 GMT  
		Size: 200.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b004703b77a56d2cfa96d9150f19bda6158c3a2812709b502227bce30bf14739`  
		Last Modified: Wed, 01 Nov 2023 11:37:05 GMT  
		Size: 33.3 MB (33285681 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:068d965d0c9a3d34cd14ceff2204edaba77eb7ae28de50c7dc898a35b06d5df3`  
		Last Modified: Wed, 01 Nov 2023 11:37:01 GMT  
		Size: 178.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06918003cb07739ec89ec2eb950301a64d1406c902bf937e10ae4f863bd263f7`  
		Last Modified: Thu, 02 Nov 2023 06:58:00 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c32573d8767a180a161190d79978674d7fe3dac64e5d7e9da6354cba3cd4986`  
		Last Modified: Thu, 02 Nov 2023 06:58:06 GMT  
		Size: 129.9 MB (129882193 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97f3d0c91515dc6f29c6a7f0343df86e94cc144c290ff94f7095a8a6f879e83e`  
		Last Modified: Thu, 02 Nov 2023 06:58:01 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfc092a633ee6832c22cc84311c0a59c7ca63a2ceb33092f35b8b22dd108a6ad`  
		Last Modified: Thu, 02 Nov 2023 06:58:01 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a566749e21716844d20287f2d9ae4c045ceab0b0d1a2e3767ca35c0a0e5fff5`  
		Last Modified: Thu, 02 Nov 2023 06:58:03 GMT  
		Size: 3.1 MB (3146245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b70e17263eccaacaa0949458d5a4c2a4045dc02cccb4265e18c45373b26f9a67`  
		Last Modified: Thu, 02 Nov 2023 06:58:07 GMT  
		Size: 76.0 MB (76019963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:716b694a25ff945078024bb0d1dffa82eac78a0f6381de4a2adaa2b97fbdc206`  
		Last Modified: Thu, 02 Nov 2023 06:58:02 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:377c1919d7566fec6f9f6738be6f4d367cbbec861d38461c6e37035895f45f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7582360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a516e26f13cc9ab026ce1389e544540e9dbe663b532f1e2289425d2e9338b42`

```dockerfile
```

-	Layers:
	-	`sha256:62bd25be61fac5a060f6e8e63542cb8fc95a1038f5092e4f4f873ea5d4051772`  
		Last Modified: Thu, 02 Nov 2023 06:58:00 GMT  
		Size: 7.5 MB (7546722 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:88791900f57255ad800fbf174ea7661dfcc81359d31d95907c20fedbcc1318be`  
		Last Modified: Thu, 02 Nov 2023 06:57:59 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-bookworm` - linux; s390x

```console
$ docker pull redmine@sha256:0f98d1d01c66e1d9713db39d4320ed65e2ef50d36fdfd557fd99ad27c4b2419e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269002120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aaa17ea09827bae9bb30151abb5537af1c2c76b128c7e05a2ab0bcb4e70892a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 30 Sep 2023 08:26:15 GMT
ADD file:2764e93c5bba50564937cce7bcaa7c7d3bdc3fd0d53a7bb09e6955e6fda8d7c2 in / 
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["bash"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 30 Sep 2023 08:26:15 GMT
ENV LANG=C.UTF-8
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_MAJOR=3.1
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 30 Sep 2023 08:26:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Sep 2023 08:26:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["irb"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RAILS_ENV=production
# Sat, 30 Sep 2023 08:26:15 GMT
WORKDIR /usr/src/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
ENV HOME=/home/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_VERSION=5.0.6
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.6.tar.gz
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=488fe08f37a8eb1011415922a8ea743b7f38d8a7a5f8822950a34a375dcf08ee
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 30 Sep 2023 08:26:15 GMT
COPY docker-entrypoint.sh / # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 08:26:15 GMT
EXPOSE map[3000/tcp:{}]
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ac72f5406002214602d5a625a21b606af78a78e99e377d3140a83021f7edd666`  
		Last Modified: Wed, 01 Nov 2023 00:48:04 GMT  
		Size: 27.5 MB (27512766 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c5470e6aa8f0e647418c95aeefd9a06fe474b3909bd884a19fa7bc85a295f85`  
		Last Modified: Wed, 01 Nov 2023 01:34:59 GMT  
		Size: 12.0 MB (12026526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a437add6f40e48f25af9d30197c3f6513eac55108f007d1d8a937059b144520e`  
		Last Modified: Wed, 01 Nov 2023 01:34:57 GMT  
		Size: 198.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb93dbf5ab5f6d7ec5fc8fcd29cae67cac881c8cb585048b97abbd82188d87ab`  
		Last Modified: Wed, 01 Nov 2023 01:36:20 GMT  
		Size: 32.5 MB (32541706 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:256f056611060b7567ebdbdc66ad5d4a7111cddf86289796886a19423bd8567c`  
		Last Modified: Wed, 01 Nov 2023 01:36:17 GMT  
		Size: 178.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59eaca02457a7aad2c59dbdf06b82ddb994959fc2e5d83ae6b70b40960e4fffb`  
		Last Modified: Thu, 02 Nov 2023 05:20:40 GMT  
		Size: 1.1 KB (1106 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07df6bb9181a33ec09923d8214777bf79f7f464759f4c4bff1d434d7b3be7ff0`  
		Last Modified: Thu, 02 Nov 2023 05:20:46 GMT  
		Size: 118.7 MB (118666303 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:000ffbe229aa3494df34a893fb9c52f2e184ec14dd1440148c12938338171107`  
		Last Modified: Thu, 02 Nov 2023 05:20:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18e08d53aa9c5b75960f34e5cf5e32dc7b6dc602e514c8873c4a53b9e81c7292`  
		Last Modified: Thu, 02 Nov 2023 05:20:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11dafabf3698210dfa2d2f7ead600a077be314c109678b138ae3f56665fcf915`  
		Last Modified: Thu, 02 Nov 2023 05:20:42 GMT  
		Size: 3.1 MB (3146230 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:28cec43bf65af429e2dfffbe10f02ffd2742436bebcb0040021d8f1104eecffc`  
		Last Modified: Thu, 02 Nov 2023 05:20:45 GMT  
		Size: 75.1 MB (75104830 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e58522bfb8aac7a8b3646e9d6795c3835870dc764de9ec943c3640d75ac7d2b`  
		Last Modified: Thu, 02 Nov 2023 05:20:42 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:b91474bd3cf8b9ec10e0b8121dfd922a36e56b7273dd7882f853ce9a0ab30a16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7567605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a633dfaafee143dfaede3a289e9281500c664bfce1223f931714508b6cf1c94`

```dockerfile
```

-	Layers:
	-	`sha256:f639acda9cfcfe16560f18d18e226f2cc8d52da69964ea1433969079661bd151`  
		Last Modified: Thu, 02 Nov 2023 05:20:40 GMT  
		Size: 7.5 MB (7532038 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:99755b3c37e77d4da0239dc1cb3b4e34c1f14c051d4cca8315de783ade19a1b1`  
		Last Modified: Thu, 02 Nov 2023 05:20:40 GMT  
		Size: 35.6 KB (35567 bytes)  
		MIME: application/vnd.in-toto+json
