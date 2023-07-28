## `ruby:latest`

```console
$ docker pull ruby@sha256:2921c2e49e07e298467e02a0dc5f0496786cc838cf914afd8f33252f66173427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `ruby:latest` - linux; amd64

```console
$ docker pull ruby@sha256:af8ae0243e3283e06a65d2aa63fd3ed16d831ef5d06a89c1fd8d2b99f1d46782
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.4 MB (383420259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85f595c0b8dbfae34e0b27a56ae60a926e488049ab524a2cd7331d0a3173a7`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 14:38:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 14:38:02 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 14:49:12 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 14:49:12 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 14:49:12 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 14:51:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 14:51:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 14:51:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 14:51:36 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 14:51:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 14:51:36 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94`  
		Last Modified: Fri, 28 Jul 2023 03:08:11 GMT  
		Size: 211.0 MB (211031643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d1c55965713c66c40e0cecf0c3aeb6f795937a3740aac7eac02a2dac97d62`  
		Last Modified: Fri, 28 Jul 2023 15:19:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c71b22972029a377f7c2fee19fdeae654e3cd4609137a8d8cc226f6e3584d12`  
		Last Modified: Fri, 28 Jul 2023 15:20:29 GMT  
		Size: 34.7 MB (34688053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9adccf9b3c6473a6b3917e9ba46e829e83806fb12427d0a0c98fadbbd47f804`  
		Last Modified: Fri, 28 Jul 2023 15:20:26 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; arm variant v5

```console
$ docker pull ruby@sha256:e359caa94835b6dc29e3415759b09739eb38b64c877d82e8c4fd517bd2e4eb2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.0 MB (346994504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6876acf9d34008dc55506d6531f16968f20fe73ee7860ada8dff0532d631269f`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:21 GMT
ADD file:7b6666a92b89bab40a1b4dda36930e1b5a7b9ab40ac8dadd2179767e027de097 in / 
# Thu, 27 Jul 2023 23:48:21 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:20:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 18:17:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 18:17:57 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 18:22:15 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 18:22:15 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 18:22:15 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 18:24:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 18:24:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 18:24:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 18:24:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 18:24:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 18:24:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:882ddccdc867712377829e4abe9ddf1190166c3dbdfc4cee67aafb08e253cc1f`  
		Last Modified: Thu, 27 Jul 2023 23:51:04 GMT  
		Size: 47.4 MB (47414939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f253718c89752af3d3827fa9e08b951a2eeb9e7fb65162096eff9684d21a4b38`  
		Last Modified: Fri, 28 Jul 2023 06:25:10 GMT  
		Size: 22.7 MB (22709706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54a2e1f4e1f80c2371c6fc46dad3133af5078cb0653caed09e33a1b64063c79`  
		Last Modified: Fri, 28 Jul 2023 06:25:32 GMT  
		Size: 61.6 MB (61554152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5a866effd7ea77f387ecba06a5bfadf0cd284c8edea17c32a923f080c768c1`  
		Last Modified: Fri, 28 Jul 2023 06:26:08 GMT  
		Size: 184.4 MB (184361103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea91a71aa84ce67e857596a0dc049ad7ecf6bf882d7a43fc6baa615eaf7cf26`  
		Last Modified: Fri, 28 Jul 2023 18:33:17 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7360a47f2792ea00d7af0da0057b87cffcb01babfac39bf90d32bfced17b1f87`  
		Last Modified: Fri, 28 Jul 2023 18:33:52 GMT  
		Size: 31.0 MB (30954227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42b5f99cbb67a7c8924af623a1eb0509a077c6c28d00f8eb27fbfea721573c1`  
		Last Modified: Fri, 28 Jul 2023 18:33:49 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; arm variant v7

```console
$ docker pull ruby@sha256:eed04e16851a25d6c3ae974fa35c24aaa1c1753c02ae3a4b29f2b104aa421475
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.3 MB (332262812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc5d8a19929de1823c06222215ed79c0df4e65a16fc6dedc98b955b227035ad`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:57:34 GMT
ADD file:be1c9c3d1025b24193774f5c0d5f790387924ed669771b461b2c599068512dc5 in / 
# Thu, 27 Jul 2023 23:57:35 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:58:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:22:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 15:22:47 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 15:34:36 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 15:34:36 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 15:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 15:36:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 15:36:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 15:36:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 15:36:36 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 15:36:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 15:36:36 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:f76b23045cf894a3a989a9812af93c6b2eb7169116a938d01b03e6856046fd3a`  
		Last Modified: Fri, 28 Jul 2023 00:02:46 GMT  
		Size: 45.2 MB (45232980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc5ca91792613eb694a9a6a96dea7fa075fa3d9bf6cd91997b3575293631923`  
		Last Modified: Fri, 28 Jul 2023 02:06:30 GMT  
		Size: 21.9 MB (21936835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41630b85b67c30afc21e9a68ad3a0b59c168c1955785b07d9f581d53cf5fa22c`  
		Last Modified: Fri, 28 Jul 2023 02:06:49 GMT  
		Size: 59.3 MB (59261975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87be995c0c0d16b4c091104694964428584b4ca1468ebecfc51fa60174b0e0d3`  
		Last Modified: Fri, 28 Jul 2023 02:07:22 GMT  
		Size: 175.0 MB (175010928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893fd2210f2e9818ed7c98e24e6cd3deb17fb4aeaac83b810042b4fa52ab140d`  
		Last Modified: Fri, 28 Jul 2023 16:08:34 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741e37436a50e52f8c9f7dd0c60c2f41beec4cb80143e3dba41b13c1cf6b6943`  
		Last Modified: Fri, 28 Jul 2023 16:09:38 GMT  
		Size: 30.8 MB (30819718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2b614bc64fc121ebcae6ea20479cc432fc5e4ee6a0b8904008140a005cdf6d`  
		Last Modified: Fri, 28 Jul 2023 16:09:34 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:159426664db93d4858c79cf6c8506ec9e2e73f7b2d33bac5e1d18636c2b81b14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.2 MB (374205879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5d5c41f60b61c8241640662aef30cd8e021c562595dfd140cc15860fe1640b`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:42:51 GMT
ADD file:fa545fc37115e874135945921d2cc72df8dc5b16d4354b2052717c7a57043e0d in / 
# Thu, 27 Jul 2023 23:42:51 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:36:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:37:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:03:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 10:03:14 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 10:12:03 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 10:12:03 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 10:12:03 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 10:13:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 10:13:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 10:13:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 10:13:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 10:13:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 10:13:53 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:fc9ce7290e7e014f69623715ba619a0d3488a7b6ecbf09e55e11160365691192`  
		Last Modified: Thu, 27 Jul 2023 23:45:54 GMT  
		Size: 49.6 MB (49591268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73373011d63f722a4ac6bc23ce7831a17f19e27ef530544642f060aa1d6b028b`  
		Last Modified: Fri, 28 Jul 2023 01:41:58 GMT  
		Size: 23.6 MB (23570127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dafffb02e2671e7e5cc07c996fed89f6ccc8e3276ce2dc1bbfb81502cdd795`  
		Last Modified: Fri, 28 Jul 2023 01:42:15 GMT  
		Size: 64.0 MB (63988301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cd1c60bb2c0a9bd6653d88494ac5f855634c2ec64a14cfa547ab2e257c6519`  
		Last Modified: Fri, 28 Jul 2023 01:42:45 GMT  
		Size: 202.4 MB (202421010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b219147f22d23c849ba0ee99b381384bb3315291e737c488b09d8c7ce94a462`  
		Last Modified: Fri, 28 Jul 2023 10:35:12 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7ad7cd73889f272133ef7c77310bfc64126fc0ff87f2ad1ac12dd31ebf5cab`  
		Last Modified: Fri, 28 Jul 2023 10:36:10 GMT  
		Size: 34.6 MB (34634797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498baef37bd31e63f67fa315c2f112ddae3f6cd035f3ffe5efff079b2717204a`  
		Last Modified: Fri, 28 Jul 2023 10:36:07 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; 386

```console
$ docker pull ruby@sha256:017b7f25e772619d8e3a5889118bbbb13e80909ceb2231a74d6969332871e740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.1 MB (382085427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed714c7cfd5683aec315a835beb28fb8c45bff5813366708ae170d2994a38c62`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:44 GMT
ADD file:bfd1a38bf0df9f79f82223093a7cc153dd7b622ab08d82845c29e6c6a2b63344 in / 
# Thu, 27 Jul 2023 23:38:46 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:02:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:04:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 13:16:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 13:16:16 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 13:31:05 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 13:31:05 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 13:31:05 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 13:34:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 13:34:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 13:34:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 13:34:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 13:34:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 13:34:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:7edd5f0eb761ecec3cc6497cb7ea8914684087583488efe885ab62bb56ddb33b`  
		Last Modified: Thu, 27 Jul 2023 23:42:57 GMT  
		Size: 50.6 MB (50567875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771ff57b30bb1e44cec48232f2b9d95b183cd6104fc0310512349e546d38d750`  
		Last Modified: Fri, 28 Jul 2023 09:10:55 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefdc80306ea3dd4a76cf653b56e8031ba3bea83dc15eb973ce4ff0eb769ea25`  
		Last Modified: Fri, 28 Jul 2023 09:11:19 GMT  
		Size: 66.0 MB (65972278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be755e8fc428a857c441e0da660385eae2ad7f53117d42e70c660589109593b`  
		Last Modified: Fri, 28 Jul 2023 09:12:07 GMT  
		Size: 209.9 MB (209946505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d587ecf73cfb8309e1f90faaad074f3cd4770ea5bbd320e648e5d8398fbc70c`  
		Last Modified: Fri, 28 Jul 2023 14:14:16 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e552597551d458321be024442212acb9a3c1b6e239ea178a7048505e841eba`  
		Last Modified: Fri, 28 Jul 2023 14:15:29 GMT  
		Size: 30.7 MB (30728643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb911384f66a1c10b11104f70640d807f2d6572320abe7289360cf837377bf20`  
		Last Modified: Fri, 28 Jul 2023 14:15:25 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; mips64le

```console
$ docker pull ruby@sha256:f1ac06b361645c2297c99439cc12927caa1a0186f3ead8e80de54774076eb33d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.3 MB (357333857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:039f82fddf8d33ab70d5b130593a1eefeb13ff9da1c136aaa4a9f52991d665e6`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 13:48:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 05 Jul 2023 13:48:40 GMT
ENV LANG=C.UTF-8
# Wed, 05 Jul 2023 14:42:18 GMT
ENV RUBY_MAJOR=3.2
# Wed, 05 Jul 2023 14:42:24 GMT
ENV RUBY_VERSION=3.2.2
# Wed, 05 Jul 2023 14:42:30 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Wed, 05 Jul 2023 14:53:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 05 Jul 2023 14:53:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 05 Jul 2023 14:53:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 05 Jul 2023 14:53:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 14:53:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 05 Jul 2023 14:53:41 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a976801f0e288a1695ce313557e999ec73ed5562492816ed2e559f8fadcba08`  
		Last Modified: Tue, 04 Jul 2023 14:58:59 GMT  
		Size: 189.6 MB (189594308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9809b679665e4f44cd2b5e69e765d478d9c120048d80dc6e7a0fd4af9783a`  
		Last Modified: Wed, 05 Jul 2023 16:49:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b1a84f2c5fb535859a63faf23b4845c3068ca948f0e9413b95b8fbe86a36f`  
		Last Modified: Wed, 05 Jul 2023 16:50:59 GMT  
		Size: 31.6 MB (31634958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e015b729fdd5ea641c74337531baa0689a5eaec099896c12efd4b7763e10c6a5`  
		Last Modified: Wed, 05 Jul 2023 16:50:47 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; ppc64le

```console
$ docker pull ruby@sha256:36ba9b9fd14385f8350e3157ab0909aef09029a5b05ac4edbe62d8e6894c9f88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.1 MB (395086780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cece3c88f9ef9ef3fb0d7cf3368d4709441e0a620cb7844a2d295725b1065e`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:22:41 GMT
ADD file:b20300808df8e1ce5b5ff534088c39d6b04467476af024e54545f7857f78a508 in / 
# Thu, 27 Jul 2023 23:22:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:48:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:51:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 07:54:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 07:54:11 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 08:28:11 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 08:28:14 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 08:28:17 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 08:32:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 08:32:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 08:33:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 08:33:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 08:33:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 08:33:05 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b6d31d119ff78cff1435e4eb51d8918916c2d5057cebf12b76d5352660fb90de`  
		Last Modified: Thu, 27 Jul 2023 23:28:46 GMT  
		Size: 53.5 MB (53543346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a33abb1f7b6ee01625f07108e25c720832ec763cb926abf676b8841aeff7a3`  
		Last Modified: Fri, 28 Jul 2023 01:59:03 GMT  
		Size: 25.7 MB (25680980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b3b1ad4b6d7fdd0b5ed658423ee70f16882053f8cd775f5234fe8217ad8a4a`  
		Last Modified: Fri, 28 Jul 2023 01:59:35 GMT  
		Size: 69.6 MB (69570344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4503d33f72e01ff054c51285f7dd69ccc8ee22b3074839b6c3769fa6e4553b75`  
		Last Modified: Fri, 28 Jul 2023 02:00:38 GMT  
		Size: 214.1 MB (214063296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb10e5f283848f73f239b52f422f6e6e4c718e9f8abfeeeb2f3189a4af0b98`  
		Last Modified: Fri, 28 Jul 2023 09:14:00 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95055a1306f6b627f4aa0cf5b658e04ed7ea9f888d5ab91eabe0c927a8156590`  
		Last Modified: Fri, 28 Jul 2023 09:15:31 GMT  
		Size: 32.2 MB (32228437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c7986e84b3e25b54076898886ae7e69da478f27119443cde6b21dfbc6037a2`  
		Last Modified: Fri, 28 Jul 2023 09:15:26 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:latest` - linux; s390x

```console
$ docker pull ruby@sha256:63b5b642a947685fa7d81e6ab0b01067aeb9e0b905a3f0482e305a8995508b8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.7 MB (349708171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edcfbd2a7d673ec18bc49df03bb18bc3663790b2525ba5dfc486f5358c0b2424`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 27 Jul 2023 23:46:54 GMT
ADD file:7cc985c20b5bf9e4dde7f388e4a49154bad3005c95f50de92b01ecec9212e022 in / 
# Thu, 27 Jul 2023 23:46:56 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:55:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:57:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 12:22:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 Jul 2023 12:22:35 GMT
ENV LANG=C.UTF-8
# Fri, 28 Jul 2023 12:31:49 GMT
ENV RUBY_MAJOR=3.2
# Fri, 28 Jul 2023 12:31:49 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 28 Jul 2023 12:31:49 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 28 Jul 2023 12:33:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		rustArch=; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		'amd64') rustArch='x86_64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-gnu/rustup-init'; rustupSha256='5cc9ffd1026e82e7fb2eec2121ad71f4b0f044e88bca39207b3f6b769aaa799c' ;; 		'arm64') rustArch='aarch64-unknown-linux-gnu'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-gnu/rustup-init'; rustupSha256='e189948e396d47254103a49c987e7fb0e5dd8e34b200aa4481ecc4b8e41fb929' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 Jul 2023 12:33:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 Jul 2023 12:33:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 Jul 2023 12:33:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 12:33:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 28 Jul 2023 12:33:41 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:93e4b40dfe5599c220b1b5acf9563fe87baf3eaa3fd2f0df5e8c0c6640a9d9ff`  
		Last Modified: Thu, 27 Jul 2023 23:51:59 GMT  
		Size: 47.9 MB (47922041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c098e736df62c7c1ec5d7910b09ebaa881acd0aa44d8c82aae2beb615c5fa8`  
		Last Modified: Fri, 28 Jul 2023 02:02:18 GMT  
		Size: 24.0 MB (24028836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0231d345104262f6b9c9131e53bf2671fb787b9a070f6c1eafb65fa6561a0`  
		Last Modified: Fri, 28 Jul 2023 02:02:35 GMT  
		Size: 63.1 MB (63112648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2eb3daed1c61a5c350b0eb0e5d07e8f61ffefd99d56ebdee3624e03432e3d0`  
		Last Modified: Fri, 28 Jul 2023 02:03:06 GMT  
		Size: 183.1 MB (183096451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacbc816c9b8fb65a56a6e49ad5f6d2f1a619c23c5eab5f3f8409790f364ed26`  
		Last Modified: Fri, 28 Jul 2023 12:54:48 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f2a3ebad1de9b2e710094aec9df981abae9c40d327aebc6c36752e86fcd397`  
		Last Modified: Fri, 28 Jul 2023 12:55:39 GMT  
		Size: 31.5 MB (31547817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3193654d391b9592aa0a7ead72174ebb29f5b58c134168cc2345ded51c7a5358`  
		Last Modified: Fri, 28 Jul 2023 12:55:36 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
