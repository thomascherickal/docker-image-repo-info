## `redmine:latest`

```console
$ docker pull redmine@sha256:837e77d474c1ec75f6f93c490a6b055144db0bbd76f9489f99092bdf230195e0
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
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
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redmine:latest` - linux; amd64

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

### `redmine:latest` - unknown; unknown

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

### `redmine:latest` - linux; arm variant v5

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

### `redmine:latest` - unknown; unknown

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

### `redmine:latest` - linux; arm variant v7

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

### `redmine:latest` - unknown; unknown

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

### `redmine:latest` - linux; arm64 variant v8

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

### `redmine:latest` - unknown; unknown

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

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:79a342d12595b978a5ce0c309f486b22db7384a08a76be49097beabc1484a044
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.1 MB (260074219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d7b1df80deef7624464dd8c05b044446bd69f5084ae18b20788e946e7ab4b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:34:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:34:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Nov 2023 14:34:04 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 14:43:30 GMT
ENV RUBY_MAJOR=3.2
# Tue, 21 Nov 2023 14:43:30 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 21 Nov 2023 14:43:30 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 09 Dec 2023 05:06:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='0b2f6c8f85a3d02fde2efc0ced4657869d73fccfce59defb4e8d29233116e6db' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='673e336c81c65e6b16dcdede33f4cc9ed0f08bde1dbe7a935f113605292dc800' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 09 Dec 2023 05:06:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2023 05:06:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2023 05:06:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 05:06:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 09 Dec 2023 05:06:16 GMT
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
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8919d6465a26017ec92b177b51035072448c414f8d8163dcf348f2f12cd06d6e`  
		Last Modified: Tue, 21 Nov 2023 15:08:37 GMT  
		Size: 13.4 MB (13402460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9504a6acac3baa3d526e36dfffc90f19acc360e11ac29e75b9345985cb87651`  
		Last Modified: Tue, 21 Nov 2023 15:08:33 GMT  
		Size: 199.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4528786b561a22ddd5d36a8b2bb643461aafaf10f0218e43cf1c36a3c296af89`  
		Last Modified: Sat, 09 Dec 2023 05:29:21 GMT  
		Size: 30.9 MB (30891907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e96c4b107f6a9944f61562af77c72ee43647ac7f83226fcf8ccb942456160597`  
		Last Modified: Sat, 09 Dec 2023 05:29:17 GMT  
		Size: 177.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19afd605466a8996c2a3cf95732dc81b5c1b237ff101fefc6bdca0c1c65a6590`  
		Last Modified: Tue, 19 Dec 2023 22:52:52 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a8031a9fb851de040ea26d9809113f217336b23e1c77317bc9b2ba9b067b754`  
		Last Modified: Tue, 19 Dec 2023 22:52:56 GMT  
		Size: 127.4 MB (127424016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96c8a66a2cfb41014c14889989e1d142ace52e43fda32f5419a22293cb452377`  
		Last Modified: Tue, 19 Dec 2023 22:52:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfbdf5d4b9c90bce0bbfe413c51a2dca4d61722af1ff1588e2b04d1f11709bcf`  
		Last Modified: Tue, 19 Dec 2023 22:52:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ef465f7d824e9dd0565ab41f60e22fba978247632348ff402f0136a42a08a71`  
		Last Modified: Tue, 19 Dec 2023 22:52:54 GMT  
		Size: 3.2 MB (3235253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb4d1c8929f377e7bff91784d196b440d37c0eb50858dcd19eda4b29ae04bdd9`  
		Last Modified: Tue, 19 Dec 2023 22:52:56 GMT  
		Size: 55.0 MB (54952711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f450eb6ff0a2b5df46965df3e1ede8424ef5a7c1a9b3a846f3b2024d062ae6ef`  
		Last Modified: Tue, 19 Dec 2023 22:52:54 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:latest` - unknown; unknown

```console
$ docker pull redmine@sha256:ffc159d5567ea06514200179aa56aa258eff5526c549b4a692f6e6b192ebf929
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22b8b98489fcee1acc3504751f09d0997f6eb47bf32d6905d66aa1a6ed856f5`

```dockerfile
```

-	Layers:
	-	`sha256:662f8ed4fc7cf718227c59de5a3abc9f4ca0c8a6fe1142ee6d7e30ab233a7c16`  
		Last Modified: Tue, 19 Dec 2023 22:52:52 GMT  
		Size: 35.5 KB (35479 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:latest` - linux; mips64le

```console
$ docker pull redmine@sha256:757d2ece07c73cf895dfe4e041016349cdce56e24f95cf44dedcd7e7ef2b77a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222022392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43bfd9a13658da35bb3d43dbfe8763d2245cf394a25dee3c4f0d567b836046d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:06:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:16:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:16:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:16:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:16:12 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:15:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:16:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:16:56 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:16:56 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:16:57 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:16:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 28 Apr 2021 17:23:50 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 28 Apr 2021 17:23:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 28 Apr 2021 17:23:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 28 Apr 2021 17:32:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 28 Apr 2021 17:32:16 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 28 Apr 2021 17:32:16 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 28 Apr 2021 17:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Apr 2021 17:32:17 GMT
EXPOSE 3000
# Wed, 28 Apr 2021 17:32:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308e0916de51c8816bb907b1f46847b9e4f2a4c13ad8496699a943b1cb1192b`  
		Last Modified: Sat, 10 Apr 2021 15:52:29 GMT  
		Size: 23.1 MB (23101289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aeaf82f75e03c0de4dc8cfbada529330605924f939a89eea76608b649fc61c`  
		Last Modified: Sat, 10 Apr 2021 15:52:19 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d76e50514a47201bc1e5d1ecd34cb3dd052f552ecc3327f756a2ff28e810fd`  
		Last Modified: Sat, 10 Apr 2021 19:44:24 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894c487a5a062ca596adb69a0c0d1787a83ea05390fc69a9508850fbd0a2aee`  
		Last Modified: Sat, 10 Apr 2021 19:45:32 GMT  
		Size: 90.9 MB (90869502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b429b96dcf10c532cff19eb56cbb9a41a6e88d65179724f8e8d0a175cb4775`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 1.3 MB (1257309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62845c559925cc0291a80649bdc3e23c43fc80a48a73be6a897e6247d616f7ef`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6114ea006b8a2dfe2a8229a601a2f01991affc3feec2a428b26707c99cc92`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f01e4f6aa8c93152628e6409bcb0a4ed4e58d22b339a7875b1bd1234f4dab7d`  
		Last Modified: Wed, 28 Apr 2021 17:48:29 GMT  
		Size: 3.1 MB (3058177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4586e261819cd3c8254e20ccb108035ad32d2411dafec9165f25cda31c2e5fe`  
		Last Modified: Wed, 28 Apr 2021 17:49:01 GMT  
		Size: 66.3 MB (66297696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c9d236001335e1d65b42d368a1dbced28a48f9d0c6d869a926ed579cd7c809`  
		Last Modified: Wed, 28 Apr 2021 17:48:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

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

### `redmine:latest` - unknown; unknown

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

### `redmine:latest` - linux; s390x

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

### `redmine:latest` - unknown; unknown

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
