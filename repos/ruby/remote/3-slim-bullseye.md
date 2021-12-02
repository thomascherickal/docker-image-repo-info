## `ruby:3-slim-bullseye`

```console
$ docker pull ruby@sha256:f4790bd7b88985edbfdf7d2a20bbaf5994a81b9a7d71610b6daeeb7d5fe8384b
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

### `ruby:3-slim-bullseye` - linux; amd64

```console
$ docker pull ruby@sha256:e77ed9b7cdd22f7b24ad3f35d3eaaef3477273ff77ed2798d11bc5ac95ec03c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70469611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de4e274e65e81824a30cd3cabe737d5445759212ad607768eafb0ae0544ec505`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:23:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:23:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 16:23:59 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 16:43:50 GMT
ENV RUBY_MAJOR=3.0
# Thu, 02 Dec 2021 16:43:50 GMT
ENV RUBY_VERSION=3.0.3
# Thu, 02 Dec 2021 16:43:50 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Thu, 02 Dec 2021 16:48:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 16:48:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 16:48:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 16:48:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 16:48:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 16:48:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2105ef7734bfb3176fb1731301dc8cba11560cb6f4560767dc010c7ec24bcb8a`  
		Last Modified: Thu, 02 Dec 2021 17:30:52 GMT  
		Size: 10.0 MB (9987818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6199182c39ff93c01c5170e9f8d2c667f9062af9c04ac8b7600d2f3a94ad9d19`  
		Last Modified: Thu, 02 Dec 2021 17:30:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e25cc70e5170dad486429fb021e6c2f33314f6e206da75524f8c57ddece5fa`  
		Last Modified: Thu, 02 Dec 2021 17:32:19 GMT  
		Size: 29.1 MB (29111197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92681c4aaa50b6b26985b315504865803b87ca952360a11d137bb8ac02c404d3`  
		Last Modified: Thu, 02 Dec 2021 17:32:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; arm variant v5

```console
$ docker pull ruby@sha256:59ad7289f041540927688b7b0f87bb705dbc5bd0c415248f912ec882307f3689
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65671541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f99023b33e8b6b6509f72448d7215bcea2a12870ea5fec711f7a09c6bde42a8`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 02:50:37 GMT
ADD file:738a04a17bdb9077594ad9a847333abe28216a7f04d3058718a5e21c236c24bb in / 
# Wed, 17 Nov 2021 02:50:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 20:42:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 20:42:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 20:42:40 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:03:22 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 19:54:27 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 19:54:28 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 19:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 19:59:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 19:59:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 19:59:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 19:59:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 19:59:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a960a56baa1baffbe2aa1e0c1fb02f9ee4816337d02fec259b312c409d77fafc`  
		Last Modified: Wed, 17 Nov 2021 03:06:09 GMT  
		Size: 28.9 MB (28911006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ec646f26ed3f05df453fb6e2e3b40c73e38a4b9291372a6d2a78ac858a1f8e`  
		Last Modified: Wed, 17 Nov 2021 21:58:39 GMT  
		Size: 8.6 MB (8630789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8864807b39306bec0dc767ff9c8e8466be8c6dd3add474b7200cfbe47d62aef`  
		Last Modified: Wed, 17 Nov 2021 21:58:31 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12168a13df2c0525be1548cdc779e0686474607977f284487b25e27d25dcce`  
		Last Modified: Wed, 24 Nov 2021 20:50:56 GMT  
		Size: 28.1 MB (28129372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1ee1b23f1a17ed4cdb5fd45990859144618d54335d4fc3eb14b56457dbe240`  
		Last Modified: Wed, 24 Nov 2021 20:50:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; arm variant v7

```console
$ docker pull ruby@sha256:11ec1481f81defaebbf3c2df8b5443ff9bc0ca4ba44b2455681c5e699cdca3ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62714917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcde93ad4e8f81f6c997de2ea0b47c2dfe783e22c450656b4841c2df0b8a3d1`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:43 GMT
ADD file:cd2ac52107a2ea6657f23850a4b29366309eb39fa177321e0a9fd6d58562ae80 in / 
# Wed, 17 Nov 2021 01:59:44 GMT
CMD ["bash"]
# Thu, 18 Nov 2021 08:06:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 08:06:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 18 Nov 2021 08:06:48 GMT
ENV LANG=C.UTF-8
# Thu, 18 Nov 2021 08:26:54 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 20:10:57 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 20:10:57 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 20:15:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:15:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:15:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:15:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:15:35 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b6e5ca4da96841e58eb27c88695a059e5105fad5a066de803f4b94ae4002ba66`  
		Last Modified: Wed, 17 Nov 2021 02:15:13 GMT  
		Size: 26.6 MB (26573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de383caf4b6be13cc84c3957ea84e71ae6941fee5c34724edbd3f02b6e259d21`  
		Last Modified: Thu, 18 Nov 2021 09:23:18 GMT  
		Size: 8.1 MB (8140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd55bdd7b3881ee8276f46c323d72651e33492ec42f2ab279bd9b4b55726da8`  
		Last Modified: Thu, 18 Nov 2021 09:23:12 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c2da1f4cf7a5f86a2aad9baca5fcbad76ae85cccbc4690971756a61a0d5b0a`  
		Last Modified: Wed, 24 Nov 2021 21:30:15 GMT  
		Size: 28.0 MB (28000661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4f58af691b87b6568ec94dc268ec74cd64fb59437340f9e6d963e30ec2743b`  
		Last Modified: Wed, 24 Nov 2021 21:30:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:015e154e6ef203008f41f6fd09b9104b367ed7dc64f838b770ff6975933bb136
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67670047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8610e2d1a9712eefaf39011ba9c4a8cd503946fbc53d1ce0d317c7fb1f277a`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 09:28:13 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:33:48 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 19:46:48 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 19:46:48 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 19:48:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 19:48:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 19:48:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 19:48:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 19:48:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 19:49:00 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e7c61b3570ed862ccf622879a565810a497b31d89dc9233ad74724113d49b`  
		Last Modified: Wed, 17 Nov 2021 09:51:20 GMT  
		Size: 9.0 MB (9033741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3178558649249287c5e43c28a587cbbeed84e6778a2b8067f094b1fd204fc4`  
		Last Modified: Wed, 17 Nov 2021 09:51:18 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c07607786573ca659cc4884de41ded15b66217121dab8182668487e56d7815`  
		Last Modified: Wed, 24 Nov 2021 20:27:38 GMT  
		Size: 28.6 MB (28579443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fc1c7201f2c399f1bfa8da45c9dc2843b14e24cf21c1cd1b00a0cf0cc11671`  
		Last Modified: Wed, 24 Nov 2021 20:27:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; 386

```console
$ docker pull ruby@sha256:53221beb74b8f2f081e3c6a3d7c1c5ece97725061a323ede1808d770a13a1b6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72562295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef3008c95da6015937c923a9c60cbe7300adecec57a322685e9d9d2bdecca36`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 18:34:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 18:34:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 18:34:08 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 18:43:35 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 19:44:38 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 19:44:38 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 19:48:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 19:48:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 19:48:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 19:48:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 19:48:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 19:48:02 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce94587ba4d01f22979518292068728c3fe52b250995e88adf9de2750201e1`  
		Last Modified: Wed, 17 Nov 2021 19:16:43 GMT  
		Size: 12.0 MB (11991101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eb951ef45c6f88babb7a5cc983a375ce043d6a24b9760459f4426f7504d49f`  
		Last Modified: Wed, 17 Nov 2021 19:16:37 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9a4aa7f77f9026ac7626f21171dfaf0a9c5a514f9c6729ce0a1e9bf69b9df3`  
		Last Modified: Wed, 24 Nov 2021 20:44:53 GMT  
		Size: 28.2 MB (28190136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217e80917bab24e7662a1d0d3baa9d4346877c53c67df68e0d58f1e092c0bc66`  
		Last Modified: Wed, 24 Nov 2021 20:44:50 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; mips64le

```console
$ docker pull ruby@sha256:d1037d766e60dccdebf531b863701e5cceeacb9952a498f3a0ae651d40a4bbe4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68710140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e5e2a6892ca2f22df33a67cfe71d8438e32b6398d6c5823b688d3860974f81b`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 16:13:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 16:13:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 16:13:26 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 16:55:49 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 20:25:00 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 20:25:00 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 20:35:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 20:35:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 20:35:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 20:35:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 20:35:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 20:35:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daf9364bca19730fd376cee2e644be3ca7680c6ae60f52294b4cc0851784e88`  
		Last Modified: Wed, 17 Nov 2021 18:32:15 GMT  
		Size: 9.8 MB (9828625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed77ad062c1a155ca0fa2a3b52915d62edd070b077612640175e4de19b11bf3`  
		Last Modified: Wed, 17 Nov 2021 18:32:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e358ca35812ef7eb458aafae72b58070b434f989fa944732f32dabc4843939`  
		Last Modified: Wed, 24 Nov 2021 22:02:21 GMT  
		Size: 29.3 MB (29250785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e0adb72ff354a199f7312fae0239497ec2bf05d424a92a370de90748931377`  
		Last Modified: Wed, 24 Nov 2021 22:02:09 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; ppc64le

```console
$ docker pull ruby@sha256:8f0d0ee54e23adbf9e2a0289dedaae9f49d7e89b0529d0b38da6f25e839700c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75311544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df91c00b110b4b5866ec0dac691eee1cacd49ce94599d09f3d9a9d01dd9c60c2`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 17 Nov 2021 03:28:22 GMT
ADD file:5ed330f0fe1328f694fcaefb961cf4da4d8a4ff03100b21af718b69316168706 in / 
# Wed, 17 Nov 2021 03:28:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:04:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:04:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 17 Nov 2021 13:04:42 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 13:27:35 GMT
ENV RUBY_MAJOR=3.0
# Wed, 24 Nov 2021 22:54:49 GMT
ENV RUBY_VERSION=3.0.3
# Wed, 24 Nov 2021 22:54:51 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Wed, 24 Nov 2021 23:00:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Nov 2021 23:00:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Nov 2021 23:00:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Nov 2021 23:00:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 23:00:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Nov 2021 23:00:49 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:258ff2a13858db8f51b65662e02137c0abcfd2528ca73e92b7a40061d938fb1e`  
		Last Modified: Wed, 17 Nov 2021 03:54:34 GMT  
		Size: 35.3 MB (35271382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd7d73cc9ef1ada2ee571fe603e1a6d6851c986db8d3bd27af6b84d4981f9a`  
		Last Modified: Wed, 17 Nov 2021 14:29:46 GMT  
		Size: 10.5 MB (10472208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735958df33ff056fdd4b0f8f8800361bb917843f910c8a6ae9da9d44f769d601`  
		Last Modified: Wed, 17 Nov 2021 14:29:30 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538b98bd955859e9f76547d795796e1a14df3fb1119692d652491927c8cb372`  
		Last Modified: Thu, 25 Nov 2021 00:15:00 GMT  
		Size: 29.6 MB (29567579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90898c41e14194965c2bb1f57ed53572513cd2926aab77c02e66c90f8862c4c`  
		Last Modified: Thu, 25 Nov 2021 00:14:55 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; s390x

```console
$ docker pull ruby@sha256:8cfb8a16676b617a65341239e744439fb8ecd6cf457e2654f9c8cb502a980b83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67765406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b1184d8398d66a106a22ac3582d22ea8f070538050e5a7190c951eb581e807`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:10:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 12:10:57 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 12:19:38 GMT
ENV RUBY_MAJOR=3.0
# Thu, 02 Dec 2021 12:19:38 GMT
ENV RUBY_VERSION=3.0.3
# Thu, 02 Dec 2021 12:19:38 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Thu, 02 Dec 2021 12:21:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 12:21:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 12:21:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 12:21:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 12:21:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 12:21:53 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ad45bc9831b0a875df976b0fb584e0cea069282d2fd94abaa8e1ee62239e3c`  
		Last Modified: Thu, 02 Dec 2021 12:43:26 GMT  
		Size: 8.9 MB (8855868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f9ebd7c7cb25cbd0b1b2471096853bcf1ebc34be816431047f52b35428c932`  
		Last Modified: Thu, 02 Dec 2021 12:43:25 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279ae4892b90be76ee2a38903e4c334cb654eee788a8e605ff372a69c1d7e8c`  
		Last Modified: Thu, 02 Dec 2021 12:44:24 GMT  
		Size: 29.3 MB (29258210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b525c142b04f1f73dd2a716f0a4eae3cfc06c1ce30659806315c5b916b953d`  
		Last Modified: Thu, 02 Dec 2021 12:44:21 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
