## `redmine:4-bullseye`

```console
$ docker pull redmine@sha256:4a3813e6b9d56671ccda89ac5c3e24d4cc5be33fa5e35642a7974a263bc5af26
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

### `redmine:4-bullseye` - linux; amd64

```console
$ docker pull redmine@sha256:e459363f4392a092cf697a26ce4ef98088cc59bc530315d3232d2302d049a51a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.3 MB (206318174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957205a2b86dfdcc36828a469d00c20016ef55a91a13d37f847d605e1a92ae44`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 10:34:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 10:34:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 10:34:08 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 11:01:18 GMT
ENV RUBY_MAJOR=2.7
# Sat, 28 May 2022 11:01:19 GMT
ENV RUBY_VERSION=2.7.6
# Sat, 28 May 2022 11:01:19 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sat, 28 May 2022 11:03:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 11:03:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 11:03:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 11:03:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 11:03:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 11:03:09 GMT
CMD ["irb"]
# Sun, 29 May 2022 04:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 29 May 2022 04:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 04:40:03 GMT
ENV RAILS_ENV=production
# Sun, 29 May 2022 04:40:03 GMT
WORKDIR /usr/src/redmine
# Sun, 29 May 2022 04:40:03 GMT
ENV HOME=/home/redmine
# Sun, 29 May 2022 04:40:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:01:19 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:01:19 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:01:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:01:22 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:02:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 02:02:06 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:02:06 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 02:02:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:02:06 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:02:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9b45ce596a6f4f1faf8c7370d2ee41943867c82cc4debc7197b6bb6dae1550`  
		Last Modified: Sat, 28 May 2022 11:08:40 GMT  
		Size: 10.0 MB (9992042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa14af4873b6b12ce5ff7b71db99fce3804547617da6ff5963fef2ee59eb478`  
		Last Modified: Sat, 28 May 2022 11:08:38 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a154d94b8c8dde803d6341f0c2c3e39ec6ae998f6bdf1492587408316b54a8`  
		Last Modified: Sat, 28 May 2022 11:12:32 GMT  
		Size: 14.6 MB (14582587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179f938bc1666f84df25f66d1020fd7adb50573785b0a2f7db1afa32d8c2b51`  
		Last Modified: Sat, 28 May 2022 11:12:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0482103cdfa997d9939c152c5a0c05f3c65f59d68db7d126728034e4d0979e83`  
		Last Modified: Sun, 29 May 2022 04:42:45 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee76ffea93830ae4d561db65280921ec06d053946ce1a4b665f22f05985bcb7`  
		Last Modified: Sun, 29 May 2022 04:43:01 GMT  
		Size: 102.0 MB (101987163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c56d4c00a00f4eb110d695f41050984e441e3f18555b2eb05e16c0717ac25`  
		Last Modified: Sun, 29 May 2022 04:42:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7721d3a3e9f4d446fed986bc6266975291000190dc2f5d5bc12680727236f208`  
		Last Modified: Sun, 29 May 2022 04:42:43 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953feee03eb930040ed99aa8a07378dd210585bd96f34c012096688721440a2c`  
		Last Modified: Wed, 22 Jun 2022 02:06:42 GMT  
		Size: 3.1 MB (3066345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa14b6688410ef830b0d2a943d044e7a7205dc1551ddc05df644e848abae997`  
		Last Modified: Wed, 22 Jun 2022 02:06:46 GMT  
		Size: 45.3 MB (45306520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24db7a15619c46fae4e87ee28bd29eac2c2b0d57e9663b98a7f6df558f5c3454`  
		Last Modified: Wed, 22 Jun 2022 02:06:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:67f6471f847e402cef7ae828f40aceda689742800d919bfda64e51bb3086d0dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203689871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2676531993e388a250c0e3b503b4d16cbb8b19f8a0b072fad881dc7a09e4e4f4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:25:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:25:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 18:25:16 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 19:26:19 GMT
ENV RUBY_MAJOR=2.7
# Sat, 28 May 2022 19:26:19 GMT
ENV RUBY_VERSION=2.7.6
# Sat, 28 May 2022 19:26:20 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sat, 28 May 2022 19:30:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 19:30:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 19:30:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 19:30:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 19:30:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 19:30:50 GMT
CMD ["irb"]
# Sun, 29 May 2022 05:09:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 29 May 2022 05:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 05:11:12 GMT
ENV RAILS_ENV=production
# Sun, 29 May 2022 05:11:12 GMT
WORKDIR /usr/src/redmine
# Sun, 29 May 2022 05:11:13 GMT
ENV HOME=/home/redmine
# Sun, 29 May 2022 05:11:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 01:09:19 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 01:09:19 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 01:09:20 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 01:09:26 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 01:15:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 01:15:12 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 01:15:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 01:15:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 01:15:13 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 01:15:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1d586d125e6bafba77551671dc44d963f57b568ab4ace206c5d0b4528440c1`  
		Last Modified: Sat, 28 May 2022 19:45:23 GMT  
		Size: 8.6 MB (8633603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ba6d77f98405f10e5bb5103a4067d822871ed8540489d0bf5011a3333e54a5`  
		Last Modified: Sat, 28 May 2022 19:45:16 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7406fa70056e3c32020d750a2daa7d67058292d56ed74735ed42ecda29f6864`  
		Last Modified: Sat, 28 May 2022 19:51:58 GMT  
		Size: 13.9 MB (13913198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca283bf40a08892f126ebda67df5d23e7d618429e8ff3182638afa35bc376f6`  
		Last Modified: Sat, 28 May 2022 19:51:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b5aadc362e5a154368037d91efc64131f85d571a30d84449628d4df11abf5`  
		Last Modified: Thu, 09 Jun 2022 18:02:43 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3daa36e5f3671c86b4ff0c6d782a1d8576c6aaaa8bf426d58517fbde4d2fa7a3`  
		Last Modified: Thu, 09 Jun 2022 18:03:50 GMT  
		Size: 97.0 MB (96957661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a05d476209a71e2b3daadc9b15c1ea40a7d910604848a9e182b51eacd13715`  
		Last Modified: Thu, 09 Jun 2022 18:02:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210372199699cfdb442b279755fc87d0d7084b492d97f308620cadb1a03cc1c4`  
		Last Modified: Thu, 09 Jun 2022 18:02:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8061a307e8b3b1edc55088cb1b3ffd10f709b2b0e7389afab6a1be5225eba8`  
		Last Modified: Wed, 22 Jun 2022 01:17:41 GMT  
		Size: 3.1 MB (3066332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed371bbfa464ba2d11e5440228dcc70e61aaa9a884ecf2911e12601902801c4`  
		Last Modified: Wed, 22 Jun 2022 01:18:03 GMT  
		Size: 52.2 MB (52193375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5db2e64d8bacccb2000874f6c38a481cfe8c5011b933c039856b5746a529b35`  
		Last Modified: Wed, 22 Jun 2022 01:17:37 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:43bf34c80591ab0efee8e1a1ec3645c77cf96e09a24cc5d55d534259bde2186f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.6 MB (196623592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:525eced5bcbc242b1825f3868b45fd4faeed4f9b6f1f8f3371a429eb2f4da3e8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 04:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 04:39:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 29 May 2022 04:39:10 GMT
ENV LANG=C.UTF-8
# Sun, 29 May 2022 05:38:46 GMT
ENV RUBY_MAJOR=2.7
# Sun, 29 May 2022 05:38:46 GMT
ENV RUBY_VERSION=2.7.6
# Sun, 29 May 2022 05:38:47 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sun, 29 May 2022 05:43:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 29 May 2022 05:43:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 29 May 2022 05:43:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 29 May 2022 05:43:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 May 2022 05:43:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 29 May 2022 05:43:14 GMT
CMD ["irb"]
# Thu, 09 Jun 2022 17:58:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 09 Jun 2022 18:00:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Jun 2022 18:00:07 GMT
ENV RAILS_ENV=production
# Thu, 09 Jun 2022 18:00:07 GMT
WORKDIR /usr/src/redmine
# Thu, 09 Jun 2022 18:00:08 GMT
ENV HOME=/home/redmine
# Thu, 09 Jun 2022 18:00:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 03:42:45 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 03:42:46 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 03:42:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 03:42:52 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 03:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 03:48:14 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 03:48:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 03:48:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 03:48:15 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 03:48:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9487628df66c5826724628aa58ae57e6636be8629f9829dc4e96a5a9d5e049`  
		Last Modified: Sun, 29 May 2022 06:00:00 GMT  
		Size: 8.1 MB (8143589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2b6d861929463b9f8a7f42db89641ba39425838c4f6eef5bbc890b5b0d2538`  
		Last Modified: Sun, 29 May 2022 05:59:53 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba51b5347b1465872a94ec50ca3a5ab3d9dd39138d7b3442c357467761c8aacb`  
		Last Modified: Sun, 29 May 2022 06:06:42 GMT  
		Size: 13.8 MB (13785143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022654e46e5b0a92bf1bea82cfa137562ebcba1308c9d80b12af8bc65c058d2f`  
		Last Modified: Sun, 29 May 2022 06:06:35 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960ee20e0c7cd63009bb0b009e6499f69a1a00fb5c8cbb707432e38645dd53e4`  
		Last Modified: Thu, 09 Jun 2022 18:10:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac153ce6a228fd90c4db9884c47d6753793b2e5f8dbee1a01e9713822277b84`  
		Last Modified: Thu, 09 Jun 2022 18:11:03 GMT  
		Size: 93.1 MB (93106533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77554da273c09a86a37cd5bf8bef8a4290b6f99ad337759dc9952247b61f2411`  
		Last Modified: Thu, 09 Jun 2022 18:10:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6941c7f9f64e21e9097eeca857b9864ef89b2bb913a698f58d4a1982073d29a`  
		Last Modified: Thu, 09 Jun 2022 18:10:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8806416df48078693b9406def961fd7488a1367a0ef665d3c98a5cf57010c884`  
		Last Modified: Wed, 22 Jun 2022 03:59:10 GMT  
		Size: 3.1 MB (3066344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe79137a3b0656092f4affda51ec9694f40e7851b004f1a37c80f81d52911bc`  
		Last Modified: Wed, 22 Jun 2022 03:59:30 GMT  
		Size: 51.9 MB (51941500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f1d2ce371f833c10684a265f4ccf8bfbd5cba95565aea3eed5c011468812d7`  
		Last Modified: Wed, 22 Jun 2022 03:59:06 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:2117e95e579fd6c0932b18e971dad5badeb27bfccf86a58a8944494191729a59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200911447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d49eb843ab5ca51324bcf0e195904f7645f2f6a4eff093b396c39607e983e1c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:44:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:44:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 09:44:03 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 10:01:20 GMT
ENV RUBY_MAJOR=2.7
# Sat, 28 May 2022 10:01:21 GMT
ENV RUBY_VERSION=2.7.6
# Sat, 28 May 2022 10:01:22 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sat, 28 May 2022 10:03:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 10:03:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 10:03:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 10:03:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 10:03:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 10:03:08 GMT
CMD ["irb"]
# Sun, 29 May 2022 00:18:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 29 May 2022 00:19:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 00:19:06 GMT
ENV RAILS_ENV=production
# Sun, 29 May 2022 00:19:07 GMT
WORKDIR /usr/src/redmine
# Sun, 29 May 2022 00:19:07 GMT
ENV HOME=/home/redmine
# Sun, 29 May 2022 00:19:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:57:45 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:57:46 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:57:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:57:50 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:58:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 02:58:36 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:58:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 02:58:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:58:39 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:58:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5abc6c8ae3d2742ede1d048644d94b8645f342236c0e9285c55851606b981f`  
		Last Modified: Sat, 28 May 2022 10:08:21 GMT  
		Size: 9.0 MB (9035742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8466cad9c45d3ea149cf3b39478c4b52b84d589aaba5b3cd835d5edf07b84523`  
		Last Modified: Sat, 28 May 2022 10:08:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe0a40d804592ebf37e48d2a541db01f9c0ed29c2dddec4f81e536d2ea76614`  
		Last Modified: Sat, 28 May 2022 10:11:07 GMT  
		Size: 14.2 MB (14180997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2da6121ce88694d7050d19ad6709e89fce9f9cd13960efe6805e193b280816`  
		Last Modified: Sat, 28 May 2022 10:11:06 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a52fa2ec9489e6497c8c187b97c1303c708a4516557870df0e5fc1ca825657a`  
		Last Modified: Sun, 29 May 2022 00:22:18 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c79da22a2f64e9dc1e427ee8ef4db8df34840af42952eee24872cfca5504332`  
		Last Modified: Sun, 29 May 2022 00:22:34 GMT  
		Size: 99.8 MB (99761700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b73625b59626be3c3095ef8902ec27dd09d8260bab029415b2edb1d4d07a2b`  
		Last Modified: Sun, 29 May 2022 00:22:16 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03125f001f8f93d8e99863f2231f6b3e89e828cd476f4526ed64552c14878a4`  
		Last Modified: Sun, 29 May 2022 00:22:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279df07205d608b14e3c00e65662ae03476e49f0df1e58d8b2751893a4e9372`  
		Last Modified: Wed, 22 Jun 2022 03:03:54 GMT  
		Size: 3.1 MB (3066506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01ff588b759d15753472ace6151efca26cf7589d2e4e9a87043b2b4710394b5`  
		Last Modified: Wed, 22 Jun 2022 03:03:59 GMT  
		Size: 44.8 MB (44796747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e3a29955f656ad1f338c633f9b287f013ce6085c97c4516cc455154a1cdbf4`  
		Last Modified: Wed, 22 Jun 2022 03:03:53 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; 386

```console
$ docker pull redmine@sha256:3346bc09795a3895a1f648529a5e9e1fce2437c9c460e668bccac2ac89fd82a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.4 MB (209378465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4c0dc4ba96aa42542fe0c546c4bebd6edd4dcf351e5b9c1e3c3298d5ea12c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:20:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:20:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jun 2022 14:20:54 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 14:48:49 GMT
ENV RUBY_MAJOR=2.7
# Thu, 23 Jun 2022 14:48:50 GMT
ENV RUBY_VERSION=2.7.6
# Thu, 23 Jun 2022 14:48:51 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Thu, 23 Jun 2022 14:50:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jun 2022 14:50:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jun 2022 14:50:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jun 2022 14:50:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 14:50:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jun 2022 14:50:40 GMT
CMD ["irb"]
# Thu, 23 Jun 2022 19:26:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 23 Jun 2022 19:26:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 19:26:33 GMT
ENV RAILS_ENV=production
# Thu, 23 Jun 2022 19:26:33 GMT
WORKDIR /usr/src/redmine
# Thu, 23 Jun 2022 19:26:34 GMT
ENV HOME=/home/redmine
# Thu, 23 Jun 2022 19:26:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 23 Jun 2022 19:26:36 GMT
ENV REDMINE_VERSION=4.2.7
# Thu, 23 Jun 2022 19:26:37 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Thu, 23 Jun 2022 19:26:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Thu, 23 Jun 2022 19:26:42 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 23 Jun 2022 19:27:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 19:27:27 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 23 Jun 2022 19:27:28 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 23 Jun 2022 19:27:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jun 2022 19:27:29 GMT
EXPOSE 3000
# Thu, 23 Jun 2022 19:27:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecc94736fb3ebe47cbc2d7c05d29dd7d597d82fb465aba483363d9020158522`  
		Last Modified: Thu, 23 Jun 2022 14:58:13 GMT  
		Size: 11.8 MB (11789428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab703ae1bcca1b3971fe42e9524647c99fd9950921459c265c05ae28237ba7d`  
		Last Modified: Thu, 23 Jun 2022 14:58:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7eac15d6452feed78c6ae13ed874f0bd1bc3ae26ce2967d7a25d0897947bee`  
		Last Modified: Thu, 23 Jun 2022 15:03:14 GMT  
		Size: 13.7 MB (13671190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215fef94d94d2e104bea660491830c73c3d956f6ca738158d095765efa41ba9b`  
		Last Modified: Thu, 23 Jun 2022 15:03:10 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb760d75745706ed42339dc023eac7994eedf481840f4f65ebe7ca29d5ab6c`  
		Last Modified: Thu, 23 Jun 2022 19:29:45 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d340d8889ce2cf4ff5f29f00e33348a0270952509ea8d3819d58ef9953b0b83e`  
		Last Modified: Thu, 23 Jun 2022 19:30:00 GMT  
		Size: 103.3 MB (103322437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f571035689523e81e1f27062e117ea2edb26709d099123b97d6cbfc8db648d06`  
		Last Modified: Thu, 23 Jun 2022 19:29:43 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa5d1765d02291d63aeb7617b318188553cd2aba2e9c4c405410ceff658265a`  
		Last Modified: Thu, 23 Jun 2022 19:29:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6c9b9f0263e4c44ba9957ac96036bbf149547f8889fd8dc79e2ebb6beffa7`  
		Last Modified: Thu, 23 Jun 2022 19:29:44 GMT  
		Size: 3.1 MB (3066508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf8aa5b21f9f247ba191bfabfc59bc6b96565bc57a3c80f7be1654bab9e9b9`  
		Last Modified: Thu, 23 Jun 2022 19:29:49 GMT  
		Size: 45.1 MB (45134684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d1d32591a407838dc597a7e5022aee77eed402b9565aafb7d53f6ff03c5297`  
		Last Modified: Thu, 23 Jun 2022 19:29:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:0121301c8827dd5184649e9d4cc4341e9aa0e31584cc97aba03f1d9a3bcaf1ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.4 MB (225379674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d875844a173a88ab75df08506cb01e738f470817e4d246454aa07303c405119c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:48:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:48:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 18:48:28 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 20:12:27 GMT
ENV RUBY_MAJOR=2.7
# Sat, 28 May 2022 20:12:30 GMT
ENV RUBY_VERSION=2.7.6
# Sat, 28 May 2022 20:12:33 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sat, 28 May 2022 20:23:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 20:23:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 20:23:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 20:23:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 20:23:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 20:23:44 GMT
CMD ["irb"]
# Thu, 09 Jun 2022 17:36:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 09 Jun 2022 17:41:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Jun 2022 17:41:11 GMT
ENV RAILS_ENV=production
# Thu, 09 Jun 2022 17:41:16 GMT
WORKDIR /usr/src/redmine
# Thu, 09 Jun 2022 17:41:18 GMT
ENV HOME=/home/redmine
# Thu, 09 Jun 2022 17:41:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 04:28:06 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 04:28:09 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 04:28:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 04:28:31 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 04:32:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 04:32:55 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 04:32:58 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 04:33:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 04:33:05 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 04:33:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81884ca0c398bb34d3d4882e21f8a008dcfd204691c1ee0405a27eecb43bc4bc`  
		Last Modified: Sat, 28 May 2022 20:40:44 GMT  
		Size: 10.5 MB (10477380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c5682fac81b7091f490a757d20fa5f676bc656e3b601fa0e6690d66627dc1`  
		Last Modified: Sat, 28 May 2022 20:40:42 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477eacdbb20acc35f31699084e26f40f6c695848e7eb10176628ca3165045353`  
		Last Modified: Sat, 28 May 2022 20:46:01 GMT  
		Size: 15.1 MB (15053732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d178ed75913386b2843fdc10d49f62b3ca0c9d54c0121328e62abfeb6a1d16c`  
		Last Modified: Sat, 28 May 2022 20:27:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce071adc3ed03aa25464b26f4ac1a62d46fa99b77a110de10d3bdba040738ce`  
		Last Modified: Thu, 09 Jun 2022 17:50:54 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41724cf4f3845ae9a81ebd2611794b6dd3cf0b6f2acb936b2fc7aac5c8b2b7d8`  
		Last Modified: Thu, 09 Jun 2022 17:51:13 GMT  
		Size: 107.5 MB (107489352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51064b103429451adcb07e0a730297ca359e3223e040a438c9a33979458eae43`  
		Last Modified: Thu, 09 Jun 2022 17:50:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26929a6d153aeaeb14f686c89832843747aedab2eb6fb20a6f1a202c1ff5689d`  
		Last Modified: Thu, 09 Jun 2022 17:50:50 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc1deee5071a3b45e034f1a566f0cd43ba78de178be91bacf547076cfff700a`  
		Last Modified: Wed, 22 Jun 2022 04:41:20 GMT  
		Size: 3.1 MB (3066333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63e4c96c499a4b96374bfcb86aa68811d75f6f2c5013ca73ffd1a3edb709543`  
		Last Modified: Wed, 22 Jun 2022 04:41:26 GMT  
		Size: 54.0 MB (54001936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d42e1a62e0b0be3d185c780282be444082ee876129370313cad7d8ab1888b1`  
		Last Modified: Wed, 22 Jun 2022 04:41:19 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:989ff68a0032ecdbdab0354cf0bcfe747577b2a12224a5410c24797191504ec5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.7 MB (208733172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac32f0fb97417d9be2649385521e0c189ea23150f14daa8a9cc19d26a8a6ed77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 14:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:32:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 14:32:10 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 15:23:26 GMT
ENV RUBY_MAJOR=2.7
# Sat, 28 May 2022 15:23:26 GMT
ENV RUBY_VERSION=2.7.6
# Sat, 28 May 2022 15:23:26 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Sat, 28 May 2022 15:26:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 15:26:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 15:26:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 15:26:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 15:26:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 15:26:47 GMT
CMD ["irb"]
# Thu, 09 Jun 2022 17:46:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 09 Jun 2022 17:46:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Jun 2022 17:47:03 GMT
ENV RAILS_ENV=production
# Thu, 09 Jun 2022 17:47:04 GMT
WORKDIR /usr/src/redmine
# Thu, 09 Jun 2022 17:47:04 GMT
ENV HOME=/home/redmine
# Thu, 09 Jun 2022 17:47:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:17:47 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:17:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:17:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:17:50 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:19:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jun 2022 02:19:22 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:19:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 22 Jun 2022 02:19:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:19:22 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:19:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b98d0a7eeb2a2311f9983303c8b3397740754665e727cd1cd1b731cd40d429`  
		Last Modified: Sat, 28 May 2022 15:37:55 GMT  
		Size: 8.9 MB (8861008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bb8472c13e6e4c380740ae1b716bd54101db0d829386d60cc9d75676303eda`  
		Last Modified: Sat, 28 May 2022 15:37:54 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e8768f4dba79cab60f4502fb7b55b68a400ae52d33438438476d01e3aa8fd`  
		Last Modified: Sat, 28 May 2022 15:41:26 GMT  
		Size: 14.7 MB (14667092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6705904282a12e0b839c1b1730f8afb540405c19c0695cf92d14fec9d3b292a`  
		Last Modified: Sat, 28 May 2022 15:41:25 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc138f9b8ddea8e36a4cd0e372ee43d2178d6d3c62121d45a0775a7a9461fdab`  
		Last Modified: Thu, 09 Jun 2022 17:52:06 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c862dbe786e95077d902ddcf4f44deef69d5b90645ac5e1655b77b70f038d19d`  
		Last Modified: Thu, 09 Jun 2022 17:52:19 GMT  
		Size: 99.1 MB (99127829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8583acf2638f10751925c89c019bb874c31861d216fbe8321592760854ba188`  
		Last Modified: Thu, 09 Jun 2022 17:52:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267b2e26cec98f85c2bf374e741979df4e32bbc0b5c928c44595de35d1fd32c4`  
		Last Modified: Thu, 09 Jun 2022 17:52:04 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef5094438cb3eed9c1a62e8ecca2714b047c3d0c0d6532a02ecd6bf2d57f375`  
		Last Modified: Wed, 22 Jun 2022 02:23:26 GMT  
		Size: 3.1 MB (3066332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cbe4f2c22bfd18d05b869a1a3dbb78b8ac10144ce596d0aaee590809d021e2`  
		Last Modified: Wed, 22 Jun 2022 02:23:30 GMT  
		Size: 53.4 MB (53351406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1623eb0bc801b4440ed979cad315a3ccb9ffa1813c5ca93896c29a4b1189a418`  
		Last Modified: Wed, 22 Jun 2022 02:23:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
