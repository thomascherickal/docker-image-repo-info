## `redmine:4-bullseye`

```console
$ docker pull redmine@sha256:d749b623f046c6fa9ee6122711cc042cfb5f9e5ef307960b4d78014e1f9a93e8
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
$ docker pull redmine@sha256:e4a134c836c9ef223001febd98eef703cd8849487ae9db33c4831b8a0db6df1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.3 MB (206343167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4877edd8ae26ae6a9794272d789d0241ae5cafc580c28c97a8af484562d1b458`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:22:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:22:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:22:33 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:50:15 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 11:50:16 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 11:50:16 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 11:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 11:52:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 11:52:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 11:52:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:52:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 11:52:07 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:43:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:43:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:43:52 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:43:52 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:43:52 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:43:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:43:53 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 23 Aug 2022 21:43:53 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 23 Aug 2022 21:43:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 23 Aug 2022 21:43:56 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 21:44:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 21:44:39 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 21:44:39 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 21:44:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:44:40 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 21:44:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacae54ed9573db0b30f6991a5f5fd01a86a6f9d946f16e68df339e1f0837d12`  
		Last Modified: Tue, 23 Aug 2022 11:57:55 GMT  
		Size: 10.0 MB (9992553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc5a66b4b23b1b64c5ac2bf68f7b4d8de90c00d75eff7ae0edb392b9de1d969`  
		Last Modified: Tue, 23 Aug 2022 11:57:53 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03676434e323e66df1d9174fbdccca0b77fd4a8a719894c2b87c387b9f5c82d5`  
		Last Modified: Tue, 23 Aug 2022 12:01:31 GMT  
		Size: 14.6 MB (14582354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc277a5593452b1afb16049b19d8dad22387f773c9631a1a065ccd7895196977`  
		Last Modified: Tue, 23 Aug 2022 12:01:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad60341104929f3c4afad3548219962aad73e37ffd0bf21e7b591ec20a1adc0b`  
		Last Modified: Tue, 23 Aug 2022 21:46:37 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813f838840ed4472e315762f22a9da88e9c6fa37a2c1413a1b1d30d1fae6e336`  
		Last Modified: Tue, 23 Aug 2022 21:46:51 GMT  
		Size: 102.0 MB (101991461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952a3bd1ecb535ec05a5187f3a0c4b0dff1da3a98bcfd4ae15a95df525e55169`  
		Last Modified: Tue, 23 Aug 2022 21:46:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0045c24b64542435d06c42177f11bddca04af436771c1b907c5c2638a5e2c`  
		Last Modified: Tue, 23 Aug 2022 21:46:34 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea400caf0532cfbe8e39462a1be9594f566f0adc9386d17cb20f113e9ff923eb`  
		Last Modified: Tue, 23 Aug 2022 21:46:34 GMT  
		Size: 3.1 MB (3066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5ab3d0b67f5166cb3dcb96da539796549a311d81ff0ebcd522a1b3ac04faf2`  
		Last Modified: Tue, 23 Aug 2022 21:46:39 GMT  
		Size: 45.3 MB (45324656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0fc221b3d1f7a22d32f1e4c007f5c2c5264a7a787b6b0397cfa4fd3ef85c8f`  
		Last Modified: Tue, 23 Aug 2022 21:46:34 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:66fe84b8898aa64037a0f8e55f40362a4d6fe506e08c96e6b690ccf0b63d5d47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.7 MB (203690882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e3ba01a2af772f94c28ee6b7909b50b5e9a8bfbfa0f754bd4cd3f54d28085a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:14 GMT
ADD file:83fb076a50e935419eb0db2bd97477d7ed5f16aaac4c8cc35a4a69ac612df327 in / 
# Tue, 23 Aug 2022 01:17:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:58:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:58:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:58:53 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 12:30:24 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 12:30:24 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 12:30:24 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 12:34:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 12:34:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 12:34:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 12:34:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 12:34:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 12:34:27 GMT
CMD ["irb"]
# Wed, 24 Aug 2022 01:24:21 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 24 Aug 2022 01:25:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 01:25:01 GMT
ENV RAILS_ENV=production
# Wed, 24 Aug 2022 01:25:01 GMT
WORKDIR /usr/src/redmine
# Wed, 24 Aug 2022 01:25:01 GMT
ENV HOME=/home/redmine
# Wed, 24 Aug 2022 01:25:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 24 Aug 2022 01:25:02 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 24 Aug 2022 01:25:02 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 24 Aug 2022 01:25:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 24 Aug 2022 01:25:06 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 24 Aug 2022 01:27:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 24 Aug 2022 01:27:26 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 24 Aug 2022 01:27:27 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Wed, 24 Aug 2022 01:27:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 24 Aug 2022 01:27:27 GMT
EXPOSE 3000
# Wed, 24 Aug 2022 01:27:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:74eb5afab626122970f8620ac001fcc4a200725acb05519b85aba47a38bf1016`  
		Last Modified: Tue, 23 Aug 2022 01:22:44 GMT  
		Size: 28.9 MB (28917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f98527654c0f97c71fec685c51d227394a931bd5ca18cee85555653d96680a`  
		Last Modified: Tue, 23 Aug 2022 12:37:42 GMT  
		Size: 8.6 MB (8634282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6261cab4f885273b0bdc7d23546f8b164451b58fca7a1aa43c9fe3b92a236`  
		Last Modified: Tue, 23 Aug 2022 12:37:38 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04abbb25c8dfb560ec64e07f0c5bae84783f747163616dbcea3865834f8e0f2`  
		Last Modified: Tue, 23 Aug 2022 12:40:49 GMT  
		Size: 13.9 MB (13913041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b088f90831bce776ca5908d76cad69299ac50f77859386b521bf90af74c117`  
		Last Modified: Tue, 23 Aug 2022 12:40:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492e6aa9d8552fdb112333fdb71887ad3e6a328673b1c52852ff1318ad6ad214`  
		Last Modified: Wed, 24 Aug 2022 01:29:28 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a29578a42ef291b62b16f7276a720110e70ce5d465c344db0a88c384cd115b`  
		Last Modified: Wed, 24 Aug 2022 01:29:54 GMT  
		Size: 97.0 MB (96962567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60cb1e4f4878ce6481fcb4a02adff5b3a0d0f1f9f2445431406a76bb0d139cb`  
		Last Modified: Wed, 24 Aug 2022 01:29:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914b125fdda337a454679a1fc05eca8e7b6d17590ce69aa20ea845c71a73c0e`  
		Last Modified: Wed, 24 Aug 2022 01:29:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25b1d1e82116e8d4cbb74688512f1d52627760f5d65a4c0095df3c8111edd29`  
		Last Modified: Wed, 24 Aug 2022 01:29:27 GMT  
		Size: 3.1 MB (3066346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6631944cf536a503c6f3b5083083178080208c30b815661bf820fa9652e3c80b`  
		Last Modified: Wed, 24 Aug 2022 01:29:38 GMT  
		Size: 52.2 MB (52193099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b488a07cfe80563853ae5ab0405eddcc3f0f958f998438db0a47506d9673f77`  
		Last Modified: Wed, 24 Aug 2022 01:29:25 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:77e4b13d546537bfdb80bf95ce33d2a3678c6db2a7aeb958375cdb2ed600321e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.6 MB (196635820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88abe26d45cfe71c2b074f64580b1a4f3de4e3db430114208aea0871800c2b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Wed, 24 Aug 2022 13:36:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 13:36:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 24 Aug 2022 13:36:15 GMT
ENV LANG=C.UTF-8
# Wed, 24 Aug 2022 14:19:13 GMT
ENV RUBY_MAJOR=2.7
# Wed, 24 Aug 2022 14:19:13 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 24 Aug 2022 14:19:13 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 24 Aug 2022 14:21:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Aug 2022 14:21:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Aug 2022 14:21:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Aug 2022 14:21:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 14:21:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Aug 2022 14:21:51 GMT
CMD ["irb"]
# Thu, 25 Aug 2022 12:36:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 25 Aug 2022 12:37:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 25 Aug 2022 12:37:24 GMT
ENV RAILS_ENV=production
# Thu, 25 Aug 2022 12:37:24 GMT
WORKDIR /usr/src/redmine
# Thu, 25 Aug 2022 12:37:24 GMT
ENV HOME=/home/redmine
# Thu, 25 Aug 2022 12:37:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 25 Aug 2022 12:37:25 GMT
ENV REDMINE_VERSION=4.2.7
# Thu, 25 Aug 2022 12:37:25 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Thu, 25 Aug 2022 12:37:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Thu, 25 Aug 2022 12:37:29 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 25 Aug 2022 12:40:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 25 Aug 2022 12:40:30 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 25 Aug 2022 12:40:30 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Thu, 25 Aug 2022 12:40:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 25 Aug 2022 12:40:30 GMT
EXPOSE 3000
# Thu, 25 Aug 2022 12:40:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b939aeabdac58fed26289eddd6831a56e2a2311739a2f8f65eb1a125da1bd4c6`  
		Last Modified: Wed, 24 Aug 2022 14:31:25 GMT  
		Size: 8.1 MB (8144135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc604ffe1810141fcd49ce49f060e1a937aa4aaf063b98fa03839489a433225c`  
		Last Modified: Wed, 24 Aug 2022 14:31:22 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd07f3b7750e629b39cdd2bbd246c603276e09b3fc575f84ea1af6a2c593df7`  
		Last Modified: Wed, 24 Aug 2022 14:36:23 GMT  
		Size: 13.8 MB (13785108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbb71b728d4c0c8a43a206028fe075814e174e5dc835e96ad1ed2323514c9d7`  
		Last Modified: Wed, 24 Aug 2022 14:36:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2544a71fb116945c4279a2923c616ae311a14991ffa4540f5dca933997148`  
		Last Modified: Thu, 25 Aug 2022 12:43:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6237f6bc94b6aedf2d09ae390837a117f6487ec9ddff3e07e1c0910e9d04dd7`  
		Last Modified: Thu, 25 Aug 2022 12:43:52 GMT  
		Size: 93.1 MB (93112496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d292af18532cfd771076f03dba3570be232171e1da5392d779f88fa9d4bb192d`  
		Last Modified: Thu, 25 Aug 2022 12:43:21 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ef8d57ae50f47b999bf861a6051cc10bc82652ec281be263ac914b8eae3eac`  
		Last Modified: Thu, 25 Aug 2022 12:43:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91f684f2ad60eb72c426291195e2f47db997fe1badd2b44e8bfef6a17b4dbf0`  
		Last Modified: Thu, 25 Aug 2022 12:43:22 GMT  
		Size: 3.1 MB (3066352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa7a808ccc88fa61f673c7642e2cb8d20c440728c7e2f60260ecf83a567a610`  
		Last Modified: Thu, 25 Aug 2022 12:43:34 GMT  
		Size: 52.0 MB (51951699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd17b0b67f3bea5d90e2bcd0e45b800ce57a42646f385309ea9fc6904dace4d8`  
		Last Modified: Thu, 25 Aug 2022 12:43:21 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:f8f805340f599927a1694e59ca8bf47d9f967d2859737dc1968901d29efcf3b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200919278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b59eee3dd0db55576c1c859d750ec0526df438be4274d8c2294ac98c15ffc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:33:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:33:55 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 12:01:21 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 12:01:22 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 12:01:23 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 12:03:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 12:03:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 12:03:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 12:03:09 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 12:03:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 12:03:11 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 23:19:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 23:19:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 23:19:40 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 23:19:41 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 23:19:41 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 23:19:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 23:19:43 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 23 Aug 2022 23:19:44 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 23 Aug 2022 23:19:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 23 Aug 2022 23:19:50 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 23:20:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 23:20:35 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 23:20:36 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 23:20:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 23:20:38 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 23:20:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cc3550da36460a5459ebbf17d504b8c97e8e52d83db0359a8512c068d33f74`  
		Last Modified: Tue, 23 Aug 2022 12:10:18 GMT  
		Size: 9.0 MB (9036227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d74a4c544da03abe5f36f8db322480084242dbceff103cc88b868bdbbdb7d`  
		Last Modified: Tue, 23 Aug 2022 12:10:17 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82670b8b9c5f2510a818c6003f3c5ec1920680629f000c7add21168528f93ea4`  
		Last Modified: Tue, 23 Aug 2022 12:14:43 GMT  
		Size: 14.2 MB (14181030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdeca94c95d3e10e794675f513be578e5e46819dce79ee545235d1fd64d5e17`  
		Last Modified: Tue, 23 Aug 2022 12:14:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecb780e29963c11951c67503496bfd3f69cfc567a0612efb7eeb266d3af17b6`  
		Last Modified: Tue, 23 Aug 2022 23:22:50 GMT  
		Size: 1.6 KB (1625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9555230508d916faa56ac8634578bf16d3a0d6e1577e513f06134de63b940e18`  
		Last Modified: Tue, 23 Aug 2022 23:23:05 GMT  
		Size: 99.8 MB (99757824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d864faa909a0609dedc9a7a7136636c2108b0e6cc3b14b3c4f038b62cb69c65`  
		Last Modified: Tue, 23 Aug 2022 23:22:48 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9eb0ea503a2db41fd34cf81b9bf49af2ec82779227902b349ff8120026134c1`  
		Last Modified: Tue, 23 Aug 2022 23:22:48 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbc1d8ac655e7079c821911a86d6c973012c2807dff41c816a86bd3023f1520`  
		Last Modified: Tue, 23 Aug 2022 23:22:48 GMT  
		Size: 3.1 MB (3066500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323f620b360604a564e580d277df0a972eaa43a69862778ce812e73b29fc3473`  
		Last Modified: Tue, 23 Aug 2022 23:22:53 GMT  
		Size: 44.8 MB (44809818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180239cc29637345d750270d537077f6d8ccb580ece38b7222694c74cc1e1ab9`  
		Last Modified: Tue, 23 Aug 2022 23:22:48 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; 386

```console
$ docker pull redmine@sha256:749289c6501bbc92cad2ec39b7764a8ca4d93bad681ba6e3afe8d656cdbc54c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **209.4 MB (209376004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3c12df05aacd4c8c3ea1ab27deeaccc49e531c1b10b96e49b66ac0a8d5f150`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 15:22:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 15:22:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 15:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 15:50:20 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 15:50:21 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 15:50:22 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 15:52:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 15:52:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 15:52:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 15:52:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 15:52:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 15:52:10 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:11:42 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:12:11 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:12:11 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:12:12 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:12:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:12:14 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 23 Aug 2022 21:12:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 23 Aug 2022 21:12:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 23 Aug 2022 21:12:20 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 21:13:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 21:13:05 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 21:13:07 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 21:13:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:13:08 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 21:13:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caacbddf1ff01b4681a908bdce5024b6fb9b342cabc00f76935eaa6c7724183`  
		Last Modified: Tue, 23 Aug 2022 16:00:29 GMT  
		Size: 11.8 MB (11789883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adcae00d7ed36ff5bf013ce67b134dee88eb5c11dc76c91340250b01d4cde31`  
		Last Modified: Tue, 23 Aug 2022 16:00:26 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c579a422c7c0dc7e75589caf683fa1ddeb5294a368228fe99f7f1269d4eee8`  
		Last Modified: Tue, 23 Aug 2022 16:06:07 GMT  
		Size: 13.7 MB (13671199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020a8fe1c7cc78b581994537e56b6f99e288779d88c89bd64dbb3d984712d6a`  
		Last Modified: Tue, 23 Aug 2022 16:06:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94dbc12036a9dcb5c3a0ed939f2958f51e3cabe1876139ec0e3b2c6c975907c`  
		Last Modified: Tue, 23 Aug 2022 21:15:26 GMT  
		Size: 1.6 KB (1616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29211752f681918f2cbac8adf09ed073f3eedb7b33c1e15dffacc7668370088a`  
		Last Modified: Tue, 23 Aug 2022 21:15:43 GMT  
		Size: 103.3 MB (103315790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acb0443dfd4e420864da4630178b6b3b3174487b1e687dc7f8357c73bb0a2ce`  
		Last Modified: Tue, 23 Aug 2022 21:15:23 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dce1fb77accde44320f5e00b3addb97ca1a99fd136e48c02cf1eea6dd36c861`  
		Last Modified: Tue, 23 Aug 2022 21:15:23 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb2cd9be78d1a0db2fb584ca0c1ad6d75a9c4c28fc72f9f9c85f6ebfa16edc9`  
		Last Modified: Tue, 23 Aug 2022 21:15:24 GMT  
		Size: 3.1 MB (3066509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167a30141f49811415c65f7c751605ac6695d4897e9723832d1b42c246ec1468`  
		Last Modified: Tue, 23 Aug 2022 21:15:30 GMT  
		Size: 45.1 MB (45141222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3375003d73f80a3b528fba446fd84cdb9097ca365484d26c5804e4448ea4ad`  
		Last Modified: Tue, 23 Aug 2022 21:15:23 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:577a25656f087061e8a7cfd36996f442d6303b6ea95d90fc0d1f5abd20cc04b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.4 MB (225358745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b8e3be32b912247908e5df6c0cea8348f5484101fea5cb602b9e0bd21e252a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:12:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 13:12:08 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 13:33:05 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 13:33:05 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 13:33:05 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 13:36:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 13:36:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 13:36:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 13:36:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 13:36:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 13:36:04 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 22:00:36 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 22:01:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:01:32 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 22:01:32 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 22:01:32 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 22:01:34 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 22:01:34 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 23 Aug 2022 22:01:34 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 23 Aug 2022 22:01:34 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 23 Aug 2022 22:01:39 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 22:05:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 22:05:19 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 22:05:20 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 22:05:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:05:20 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 22:05:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc1d8f5a9f0c95e449312b1ebc8beaafe22f38b7609141d3368efd9efa9221f`  
		Last Modified: Tue, 23 Aug 2022 13:40:20 GMT  
		Size: 10.5 MB (10478166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410ddc095d085f2ed44ac21e69fd3d6d462bf616dfe3a0495655b10802520283`  
		Last Modified: Tue, 23 Aug 2022 13:40:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e054897f3ef4ba84edec146accc88fb917c47dc7df696be0d5c396002d41ac6c`  
		Last Modified: Tue, 23 Aug 2022 13:43:51 GMT  
		Size: 15.1 MB (15052691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e9b509e440316281485e426af073468bc664dab7858e26ac20c2cc1b52f74d`  
		Last Modified: Tue, 23 Aug 2022 13:43:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c546360a753195bbd5b51ba507e6509ac6854df861ac7d375bbfa12efeaceb5d`  
		Last Modified: Tue, 23 Aug 2022 22:07:47 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a9c452dbdfe2c767bcf286db313e71c5011271d5b76231d130c5bd2fbbf9b8`  
		Last Modified: Tue, 23 Aug 2022 22:08:15 GMT  
		Size: 107.5 MB (107478958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fbdcba855f88fc80a74405ab157c03c11b1543f1195765604beae7dc3c5e7`  
		Last Modified: Tue, 23 Aug 2022 22:07:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ec61ea76b1113d9d42b98b9bf0d663b4a9ceb12ba9838ea8d888c17f698753`  
		Last Modified: Tue, 23 Aug 2022 22:07:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4787052373a45bd1e941cf8089ced1fc115e0aa97b7db1ad4852a67001fb4923`  
		Last Modified: Tue, 23 Aug 2022 22:07:46 GMT  
		Size: 3.1 MB (3066350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd40cc5face7bd14198364ade4b08f7e8abab50cfe229a09064ce957d824ae3`  
		Last Modified: Tue, 23 Aug 2022 22:07:53 GMT  
		Size: 54.0 MB (53993999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4020de8acd87701fd36459fa88b7b29e11d8bf2c23334d49f9433155ea9e3a1`  
		Last Modified: Tue, 23 Aug 2022 22:07:45 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:9690d9911a8bdaf915c07797a3e70f7cab6d52ba32f3e5b181faa5139fe39d5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.7 MB (208727891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49dc5c1d5e8f8b0308bf486cc403aa519f980cfa8a1a5d1a8e27163a719bcd7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 14:20:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 14:20:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 14:20:39 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 14:34:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 23 Aug 2022 14:34:12 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 23 Aug 2022 14:34:12 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 23 Aug 2022 14:35:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 14:35:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 14:35:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 14:35:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 14:35:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 14:35:42 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 22:03:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 22:03:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:04:02 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 22:04:03 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 22:04:04 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 22:04:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 22:04:06 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 23 Aug 2022 22:04:07 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 23 Aug 2022 22:04:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 23 Aug 2022 22:04:13 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 22:07:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 22:07:22 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 22:07:22 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 22:07:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:07:23 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 22:07:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677c697e370a8ab15d79be88b7de50f457ed2649f8b41f560c690bf836cb54`  
		Last Modified: Tue, 23 Aug 2022 14:39:50 GMT  
		Size: 8.9 MB (8861883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d882cb8d7fd78f1a0db12c31ee5670613d37182cb04cd8d99e2b8cce6e67103`  
		Last Modified: Tue, 23 Aug 2022 14:39:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45ea67c66d5a9220c813feb73a7def4b5eda70d6aa5203cc50f08528173670`  
		Last Modified: Tue, 23 Aug 2022 14:42:10 GMT  
		Size: 14.7 MB (14666790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8f4d044a3eca45258408f0948fab3d112ca0c05481a27032bcd359c6227f40`  
		Last Modified: Tue, 23 Aug 2022 14:42:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5d86e5912d4a2273f28c25dac0ebea83b3e45bc48fcda47dfd0647dd8bb714`  
		Last Modified: Tue, 23 Aug 2022 22:16:02 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182cee1f37d1ea42928eb85b10cf63ba02b440d347e9d3d8802de2a0c6f110b`  
		Last Modified: Tue, 23 Aug 2022 22:16:06 GMT  
		Size: 99.1 MB (99128751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911e4b6f84475dc4c7a892f14b68003644ac2a48787c968202317953d62e7f3d`  
		Last Modified: Tue, 23 Aug 2022 22:15:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee75386d5ab8bf801f93e57f5873b2640dcfe6e9a2b646b2f9d300a452a36950`  
		Last Modified: Tue, 23 Aug 2022 22:15:40 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573cb2a822343b4c62d14e8f907666fee19608f5f88cf4b43b5e35f25aee6263`  
		Last Modified: Tue, 23 Aug 2022 22:15:41 GMT  
		Size: 3.1 MB (3066353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cb56ef3efa9fa46d86ff6e55ab5b4543405f4a4ac96ce6e1a1d04055f57096`  
		Last Modified: Tue, 23 Aug 2022 22:15:45 GMT  
		Size: 53.3 MB (53349712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c340f266021c30ad0cceba7db5f475f7c2de4ba40919fd4c401493bdc623f3`  
		Last Modified: Tue, 23 Aug 2022 22:15:40 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
