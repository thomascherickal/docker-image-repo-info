## `redmine:bookworm`

```console
$ docker pull redmine@sha256:118aed72ca3b6f10993b09f8797cddeeb524d371f2b2e657232c5d0f058f62ab
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

### `redmine:bookworm` - linux; amd64

```console
$ docker pull redmine@sha256:97579ebb2058678f2951f7f18d9370c5a3edbcefde25983d1f3eb55e466acb5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258629936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896ef06eb0ee0ed655c22b998d00acab76301b192e8d3570e7fcc1b505ccd339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 16:12:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 16:12:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 16:12:02 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 16:23:48 GMT
ENV RUBY_MAJOR=3.2
# Tue, 19 Dec 2023 16:23:48 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 19 Dec 2023 16:23:48 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 19 Dec 2023 16:26:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 16:26:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 16:26:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 16:26:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 16:26:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 16:26:32 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:640cd6e8a0c52ee2a59d5f0831f4b67cd2f151ac1dff965c576d304eb111e7d0`  
		Last Modified: Tue, 19 Dec 2023 16:52:19 GMT  
		Size: 13.9 MB (13850781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea285d4807fddf184e7e184db755e2be432a9a194aaa7118518f22f78b0707aa`  
		Last Modified: Tue, 19 Dec 2023 16:52:17 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf1068ea6dc4bab3eb5b6ec8b46ae4c662660ddece16d56ba1e4a37875013eca`  
		Last Modified: Tue, 19 Dec 2023 16:53:24 GMT  
		Size: 35.0 MB (34987053 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef6d89134a781bbffb8dcf0ee66651cda14bd9b5a4bd55e99d5fee27d66fb500`  
		Last Modified: Tue, 19 Dec 2023 16:53:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e6b528abfa74c88cdd3d5011e954d87ffe6dec49246617e637a837eda436601`  
		Last Modified: Tue, 19 Dec 2023 22:52:51 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fed656d9824dd80a4b733faee6396c1235b264776e73f45dad13c4aa12cee366`  
		Last Modified: Tue, 19 Dec 2023 22:52:53 GMT  
		Size: 123.1 MB (123110778 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e3a9f9927ea3cb3d3bb9987e906cdba5cb0ab88fcdb2e7785adbc13b93215c4`  
		Last Modified: Tue, 19 Dec 2023 22:52:51 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fce53e20611b2c665d8875e3de3f23a5ad2850c1fc2cf7e471e8fd69e182d22f`  
		Last Modified: Tue, 19 Dec 2023 22:52:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33e121530f29a1b75120bf6130bffb65be92d285cc4568c05ca8966ab219812c`  
		Last Modified: Tue, 19 Dec 2023 22:52:52 GMT  
		Size: 3.2 MB (3235254 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44391f1b387f9a55d5f59f17878c2e10cfdb0e1d09f601751c55d2da45fe6589`  
		Last Modified: Tue, 19 Dec 2023 22:52:54 GMT  
		Size: 54.3 MB (54316344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59f7125163c0279aa7288f0c9cffeb76dcfc6ee2fcdd781a353d3e9196a1813a`  
		Last Modified: Tue, 19 Dec 2023 22:52:52 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:eb7067a41a68adc1436503ac6a9d85b887fda8843ad3c099046fec288ac4fecf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7588987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46b8567e00cb45818e323b45e84ff20508779b3df5e6eb39609b5b721ccecab`

```dockerfile
```

-	Layers:
	-	`sha256:c3ea6912f6ae188a2e2ae7c104b465c1bbba35922cff5f56d48d4c8fd63213ac`  
		Last Modified: Tue, 19 Dec 2023 22:52:51 GMT  
		Size: 7.6 MB (7553236 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6ed01bdef3be45907de13b9f64a01a48ec849e7dd17a5075f797e4adc1f5d4b0`  
		Last Modified: Tue, 19 Dec 2023 22:52:50 GMT  
		Size: 35.8 KB (35751 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:bookworm` - linux; arm variant v5

```console
$ docker pull redmine@sha256:7a9391b7de4d76064c36fa27386360019df551f731e54c69dd64cfc23a89e493
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.9 MB (240931673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0fe03b8b5a061a4a5959b44498da0ef527fda37b916106034fa1edead5ca91`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 12:54:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 12:54:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 12:54:10 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 13:03:59 GMT
ENV RUBY_MAJOR=3.2
# Tue, 19 Dec 2023 13:03:59 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 19 Dec 2023 13:04:00 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 19 Dec 2023 13:06:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 13:06:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 13:06:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 13:06:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 13:06:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 13:06:27 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:752832ef3f809e215d9ed3bcb63cec7e89b8e7270dc33a513e4dcac39575ad5a`  
		Last Modified: Tue, 19 Dec 2023 13:26:19 GMT  
		Size: 11.6 MB (11608266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cae72c02b9aaac8e22d19c3ae77a4a6bef3523b7a05e8f47da7497a6681f9dc`  
		Last Modified: Tue, 19 Dec 2023 13:26:17 GMT  
		Size: 200.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17290f4d4dacbc59e9efed1d196a3a798a007ffed34129726f581f3386729068`  
		Last Modified: Tue, 19 Dec 2023 13:27:29 GMT  
		Size: 31.1 MB (31056497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3058a1ca96aa8ae3dccd2c870f0940ebff728a4ba99671ce5fb8686896175bc5`  
		Last Modified: Tue, 19 Dec 2023 13:27:26 GMT  
		Size: 178.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c570b318a2611033d3a6780ab200c6f70bf07286dca8949e29fbfbbbd3581b9`  
		Last Modified: Wed, 20 Dec 2023 01:16:10 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:012e1b86c2d1aa4b55cf8c9a38f2afe52e93057fab572035adf659e9f28266ac`  
		Last Modified: Wed, 20 Dec 2023 01:16:14 GMT  
		Size: 116.6 MB (116591036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca59890ce08abec3f96fce13669b668d1c5e6312f98e2c331a1d6c55c3dee065`  
		Last Modified: Wed, 20 Dec 2023 01:16:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61bb9b1e99570812968d0e0c7a3bf76ff01e1459bd0db660e6c11720df186aeb`  
		Last Modified: Wed, 20 Dec 2023 01:16:11 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:732d6f4a6559cc748fcb1b9e59de4fea546984b4cd7a6da57fed25e05cec536d`  
		Last Modified: Wed, 20 Dec 2023 01:16:13 GMT  
		Size: 3.2 MB (3235228 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2a5cd23a35f65695d660bdd5204a43c065dfd05f813d936f1ba35afa21719a3`  
		Last Modified: Wed, 20 Dec 2023 01:16:14 GMT  
		Size: 51.6 MB (51551442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc55f3066ca7fdfc117f83f106b41d19c3e2ddcef47f46de4367f8c166e6ce81`  
		Last Modified: Wed, 20 Dec 2023 01:16:13 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:c405aeecbcdab62390ea9a7b77f9d044223daa7438c0d2e6e8c5e58429fa5e52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 KB (35689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616fb9505266d9cea8ee9b762dcad1c4114d7cefc1968b0f48937886ee60459d`

```dockerfile
```

-	Layers:
	-	`sha256:8dcff61dede7bf091378820b4d00f5283375c6d57691a532a12966642f831eda`  
		Last Modified: Wed, 20 Dec 2023 01:16:10 GMT  
		Size: 35.7 KB (35689 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:bookworm` - linux; arm variant v7

```console
$ docker pull redmine@sha256:7ff9b6347a6bba28d18dcb2fae9a6ae1a052a27edc039601a830cb45d0cf97fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.3 MB (233278007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a66a44ed417217d36829ef7c521fe6c35f06e79b3346dddaa4cb59e42524f3df`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 14:02:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 14:02:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 14:02:43 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 14:12:08 GMT
ENV RUBY_MAJOR=3.2
# Tue, 19 Dec 2023 14:12:08 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 19 Dec 2023 14:12:08 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 19 Dec 2023 14:14:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 14:14:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 14:14:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 14:14:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 14:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 14:14:11 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fdde23b75ff861ef18312860e3828e93a1be88cb9ae4964e04c18d4ea04f839d`  
		Last Modified: Tue, 19 Dec 2023 14:36:24 GMT  
		Size: 10.9 MB (10944290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2fe047ae909041d9587335359b8a53e691be80b65987e483212f06ea08d0e18b`  
		Last Modified: Tue, 19 Dec 2023 14:36:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e03cb1302122cf8f4bdc88adf13bca87af3df239bd921f5510590942cdaf0e7`  
		Last Modified: Tue, 19 Dec 2023 14:37:29 GMT  
		Size: 30.9 MB (30899770 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:747a3a0571a4f2886ff5046fc35b8e34c8a58c0c5fa8677419d59e24bb3a3b6b`  
		Last Modified: Tue, 19 Dec 2023 14:37:26 GMT  
		Size: 177.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ef0fdb35f86bcb7cf1fa7526415c42604cdfaf3ac50eb18d55ae980bf32f07a`  
		Last Modified: Wed, 20 Dec 2023 09:33:26 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc46246a7865b755da40f276fdb0f269dc862e1d4c5c06dad3abbdacfc7732eb`  
		Last Modified: Wed, 20 Dec 2023 09:33:30 GMT  
		Size: 112.1 MB (112093103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75ef8e17d2e6a3980848ec3d7109fe9a6409c7ea3ed95dffa2fcaa624b7b228f`  
		Last Modified: Wed, 20 Dec 2023 09:33:27 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18be0403804f6918193eae243874557d87b2604eb47e06fc1093671793949fda`  
		Last Modified: Wed, 20 Dec 2023 09:33:27 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2371f4758757599a69768fb507df09f5687212355b09cd31e90cdbb45cf62be6`  
		Last Modified: Wed, 20 Dec 2023 09:33:28 GMT  
		Size: 3.2 MB (3235226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b2b408b3b5fb8cc08989ab56f9232a6232c7d41ba57b93ff2ff58999e1aad957`  
		Last Modified: Wed, 20 Dec 2023 09:33:31 GMT  
		Size: 51.4 MB (51383696 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b1cb17b296889bce82c7f04a114ad1e9370d44d153182b650a1bb9cb28fd2d0`  
		Last Modified: Wed, 20 Dec 2023 09:33:28 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:4c5792b383bf4493fd090049ebd61fda0cb438a4f288a1c026c92230c5205597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7559473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa2311dfa6c2dd18388608ddf15ab9affc0e5c82e44636187354f361aed5ac04`

```dockerfile
```

-	Layers:
	-	`sha256:fc2c045039762b6b9c8ce874acd5ad54835af60787079fa1398b410ea2508bc5`  
		Last Modified: Wed, 20 Dec 2023 09:33:26 GMT  
		Size: 7.5 MB (7523568 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ae764da013536583e1581e4baa350a25906c9aab2bb97d087073cad405a792fc`  
		Last Modified: Wed, 20 Dec 2023 09:33:25 GMT  
		Size: 35.9 KB (35905 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:bookworm` - linux; arm64 variant v8

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

### `redmine:bookworm` - unknown; unknown

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

### `redmine:bookworm` - linux; 386

```console
$ docker pull redmine@sha256:491b10cc863f2ca1c2706a3e92766ea282ec83f0b156d21d0411a9c77ea6aa6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.6 MB (257564087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055fb8c02ee352d94a6215905556a194f817ba7ba24b440d606deec2adfc8c5a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:07 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 19 Dec 2023 01:39:07 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 19 Dec 2023 17:42:47 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RUBY_MAJOR=3.2
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 19 Dec 2023 17:42:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 19 Dec 2023 17:42:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 19 Dec 2023 17:42:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Dec 2023 17:42:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:852d358ffed1dcad0622de35e6faca03420c720a207af551a3e0337791df7edc`  
		Last Modified: Tue, 19 Dec 2023 23:28:20 GMT  
		Size: 13.4 MB (13399500 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fd946c3244c6fc94c8c8075176d7cb724f882536a7c0f3db64571aff76f5cd4`  
		Last Modified: Tue, 19 Dec 2023 23:28:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18c1b6eb4bd80e60ba2095328ee781feed9ec06446789e3b21c273dbb4233e63`  
		Last Modified: Tue, 19 Dec 2023 23:29:31 GMT  
		Size: 30.9 MB (30891278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70f14836322f9db703c65e083999f8d4c07a35f3192dc0cf172aa5831cc004a4`  
		Last Modified: Tue, 19 Dec 2023 23:29:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:751abef554c503f155cafd22b2009e451ebcbaa2dde90754c01c1dd09c7bdbd5`  
		Last Modified: Wed, 20 Dec 2023 00:51:55 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6526dd3917bf7319292d687b2d3d7e2ede1b58c9b5dfd19b8c75977d35fac4c6`  
		Last Modified: Wed, 20 Dec 2023 00:51:58 GMT  
		Size: 124.9 MB (124938531 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef7998295e72016a1ad1c5e51be2b79e7f240e663b36355afc81e2daf2ef2e2c`  
		Last Modified: Wed, 20 Dec 2023 00:51:56 GMT  
		Size: 140.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ced39de7ba85820255aeecd5ceae1be46ac178d2aba2136a230cde7ae9d6e7c0`  
		Last Modified: Wed, 20 Dec 2023 00:51:56 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a8cc72c6984f962bf5c55746f64c42cb79d17cc6ec912b04b5e01a7c599db59`  
		Last Modified: Wed, 20 Dec 2023 00:51:57 GMT  
		Size: 3.2 MB (3235258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab49e51116ea5a7247fdd1779b19ccba7946a6bf36a646a135da0c94a112a205`  
		Last Modified: Wed, 20 Dec 2023 00:51:59 GMT  
		Size: 55.0 MB (54951896 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1850324b8c1deec7ca9c6d710838359cf72cb851f2ad001256afd8b1b2dbb05f`  
		Last Modified: Wed, 20 Dec 2023 00:51:57 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:bookworm` - unknown; unknown

```console
$ docker pull redmine@sha256:7f03f33abc7c56b86355ce936c96201152510e2907cbe0e06c1d9ec074a65d0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f077ce3b9f859e14d5ebaba4d6ef376141e396dd437b2a1c72ab03370782e2fe`

```dockerfile
```

-	Layers:
	-	`sha256:ddbda58015fcbb6e6c76f3d453ab6f56aad2527f746db3efbe7cdcd9f458ecbf`  
		Last Modified: Wed, 20 Dec 2023 00:51:55 GMT  
		Size: 35.5 KB (35479 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:bookworm` - linux; ppc64le

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

### `redmine:bookworm` - unknown; unknown

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

### `redmine:bookworm` - linux; s390x

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

### `redmine:bookworm` - unknown; unknown

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
