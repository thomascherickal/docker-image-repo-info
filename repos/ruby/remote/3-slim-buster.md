## `ruby:3-slim-buster`

```console
$ docker pull ruby@sha256:aaf31982a84c7543a44814bf3e2dc8f8512eeeda0a7d70fe8226edbbd529dc2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `ruby:3-slim-buster` - linux; amd64

```console
$ docker pull ruby@sha256:fe7a7d9b124b89851e000c76f21e2270c4953991ee2d6509d33ba72cf42b49ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (74016637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219bce62aca78edd73f7e1b99b54a071ebe1a2cc74de5467ef8f55a81585081f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 11:34:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 11:34:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 11:34:24 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 11:44:37 GMT
ENV RUBY_MAJOR=3.2
# Tue, 23 May 2023 11:44:37 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 23 May 2023 11:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 23 May 2023 11:47:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 11:47:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 11:47:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 11:47:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 11:47:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 11:47:08 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab35ad3db6e6767cc2acd3e3c94152de2ccf3136e8a2e94f9979baaa4809205`  
		Last Modified: Tue, 23 May 2023 12:06:21 GMT  
		Size: 12.6 MB (12581694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb47709c2a8683da2452935c5859890259b22e644a7f67cfdf72082f24039c89`  
		Last Modified: Tue, 23 May 2023 12:06:19 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28757a8b3f9421bbb3deac77f51ded161e2e532803f8a5cf21547e824953479`  
		Last Modified: Tue, 23 May 2023 12:07:39 GMT  
		Size: 34.3 MB (34295991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8fb1706da7b6d25e2648055926c063fbb900ba3c1b3f8bdefa836ef28bd169`  
		Last Modified: Tue, 23 May 2023 12:07:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:cfc89421ba720ffdd1277da7d34f1f1058186d6ee1e257546fe401bcec06dfa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62755030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66e4f08be724d6c532d64934f4fd1a16a20155b4b077d870736e9bf2dbc64932`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 23 May 2023 00:58:17 GMT
ADD file:fc75413703cf08c1fc3b981ebbde07494b7ad8176aadd5f3a8fb891f0c48e7b9 in / 
# Tue, 23 May 2023 00:58:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:33:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:33:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 05:33:08 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 05:38:17 GMT
ENV RUBY_MAJOR=3.2
# Tue, 23 May 2023 05:38:17 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 23 May 2023 05:38:17 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 23 May 2023 05:40:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 05:40:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 05:40:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 05:40:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 05:40:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 05:40:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:0265ca860f8350954d0667b45b48728e992970f63232c58e18fac59852acd8f2`  
		Last Modified: Tue, 23 May 2023 01:02:24 GMT  
		Size: 22.7 MB (22747412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d7d5221b059e1a1180a1ef2ef6dca32d9de4d6d62dddcde9e3418134edb25`  
		Last Modified: Tue, 23 May 2023 05:51:08 GMT  
		Size: 9.9 MB (9879314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c957d23d7c0d8ea0704e98727cbd1e3d89d9ce7b251e1e1b26a27c1b10533c`  
		Last Modified: Tue, 23 May 2023 05:51:06 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e7f8df77c5be67c26d9814734000310f9a17c5f1d954abf45412807158222`  
		Last Modified: Tue, 23 May 2023 05:51:44 GMT  
		Size: 30.1 MB (30127930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73847473e625d3a39865110203fe8e693a74795e2b302a2e41c0c185499f1be`  
		Last Modified: Tue, 23 May 2023 05:51:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:b7939507b772b7140e2da4a9c3c5493c83179327d2df22e3ab50ab3441804776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71440863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9177e2db7ceb321f7cd4da36f3ee074d0ac0a574c4b5fea203e49a4cce5f425c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 23 May 2023 00:43:28 GMT
ADD file:55a469039df0bf0e94ef7cd2d6fd355ad0c69e0e23e7921194445dd1fe281e3b in / 
# Tue, 23 May 2023 00:43:28 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:21:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 06:21:29 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 06:29:40 GMT
ENV RUBY_MAJOR=3.2
# Tue, 23 May 2023 06:29:40 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 23 May 2023 06:29:40 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 23 May 2023 06:31:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 06:31:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 06:31:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 06:31:36 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 06:31:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 06:31:37 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3ca7b6c7180eac66b9c4301084a16319f41eb7f7365bdf91bcc272bd24cb4149`  
		Last Modified: Tue, 23 May 2023 00:46:44 GMT  
		Size: 25.9 MB (25921744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10492cb94cb7315b317481770999acd28ce5527e74115b9d5abc24133982f9a0`  
		Last Modified: Tue, 23 May 2023 06:47:09 GMT  
		Size: 11.3 MB (11282085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a990726a426b3fd58648ce5842c8f482a00de76f3e657cf6e0a0ca95cf923794`  
		Last Modified: Tue, 23 May 2023 06:47:07 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04a6411b5ebefa9baa18e756cfc21ba078fe7cd5c31d6b82b562f554df5215c`  
		Last Modified: Tue, 23 May 2023 06:48:21 GMT  
		Size: 34.2 MB (34236658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c353adbf54c621ccdfebdc0299aca5ef3c0076f825a9816cd3225046c70dc5e6`  
		Last Modified: Tue, 23 May 2023 06:48:18 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; 386

```console
$ docker pull ruby@sha256:d1192f600b1bdf2aa8392a8fc79a5f6bf0ddba24669f9044d46d7d107f6895d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75458372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02f9aed305932c3e17dd77db713bcb56f1517319ba5ca8deab0327992c7b182`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:16:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:16:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 May 2023 01:16:20 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 01:24:22 GMT
ENV RUBY_MAJOR=3.2
# Tue, 23 May 2023 01:24:22 GMT
ENV RUBY_VERSION=3.2.2
# Tue, 23 May 2023 01:24:22 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Tue, 23 May 2023 01:27:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 May 2023 01:27:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 May 2023 01:27:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 May 2023 01:27:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:27:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 23 May 2023 01:27:52 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5393fea6729798b5e16fe4f454e14886b93b7e4b07c56e998c315b3ac55772`  
		Last Modified: Tue, 23 May 2023 01:43:37 GMT  
		Size: 17.2 MB (17247812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2d4328323e7718dfcd9de62989737e49af09d5db90930f8712fad0cc0b79e5`  
		Last Modified: Tue, 23 May 2023 01:43:32 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d363db5ca77ab331aae9957f4356ea160043e01302625243a253e9d851e45897`  
		Last Modified: Tue, 23 May 2023 01:44:16 GMT  
		Size: 30.4 MB (30412977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535b67e6cb0126a1d99c3a443d3f79188b5eab733bdac0a2c0815b53f4851c38`  
		Last Modified: Tue, 23 May 2023 01:44:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
