## `ruby:2-slim`

```console
$ docker pull ruby@sha256:73199788d993ee38e6cff8c90f582c9153d2fa84a20a2f025af6b55e03a4bea0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `ruby:2-slim` - linux; amd64

```console
$ docker pull ruby@sha256:588a56ff2fe0df6ee5ae7ff9583f8848ba610af35fea2c06770777d20218ab16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62484549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb332fdeafeef6a59bbd03a0f660d19ff6e24f200a47781d038cab4fa5586d5`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 18:23:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 18:23:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 18:23:20 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 18:32:28 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 18:32:29 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 18:32:29 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 18:37:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 18:37:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 18:37:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 18:37:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 18:37:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 18:37:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b853ec9f225871c979a2eaad017baf089203d44c6fdc51a163fa31a65bcf71`  
		Last Modified: Tue, 13 Oct 2020 19:08:00 GMT  
		Size: 12.5 MB (12539335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21147059b9954928941f1c99980095af839dba576d0f84ae0a525b030f552b9`  
		Last Modified: Tue, 13 Oct 2020 19:07:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6943e1e2b47b01e4666c6496503bec1e3661bcaf8500e99fe262723bc9ee70`  
		Last Modified: Tue, 13 Oct 2020 19:08:27 GMT  
		Size: 22.9 MB (22852645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cfe3b29903912b3ee8818347f7054afaf77f6c0ce91bbc179ebc810717626a`  
		Last Modified: Tue, 13 Oct 2020 19:08:22 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; arm variant v5

```console
$ docker pull ruby@sha256:ed2a02dcb442d6dfd5b2111bb6cdf2e438bd2c0c0091592efd51a313c29a3583
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57284894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7881fa64ad7222d17e6adadae0e0b2799c033427ce978ef9d56c90825df06e63`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:03:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:03:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Nov 2020 21:03:39 GMT
ENV LANG=C.UTF-8
# Tue, 17 Nov 2020 21:08:58 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Nov 2020 21:08:59 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 17 Nov 2020 21:08:59 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 17 Nov 2020 21:13:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Nov 2020 21:13:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Nov 2020 21:13:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Nov 2020 21:13:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Nov 2020 21:13:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Nov 2020 21:13:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d07e7122dd66132ed5ab7684a2a8ae49cfe80bf95fd320eb7aad98ada09e96`  
		Last Modified: Tue, 17 Nov 2020 21:32:41 GMT  
		Size: 10.3 MB (10327078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa508c59a973b7859d6139bcae74831a82db3d60842942c12f904d25c27c17b`  
		Last Modified: Tue, 17 Nov 2020 21:32:38 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e014ecd2173d84182f4f233772217c958bc135ceac6c2686c49c4fa7e81b3`  
		Last Modified: Tue, 17 Nov 2020 21:32:59 GMT  
		Size: 22.1 MB (22107130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab9232216a11a31664d63e6a56af9707c731a5eac5495980d87e703641e694b`  
		Last Modified: Tue, 17 Nov 2020 21:32:55 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; arm variant v7

```console
$ docker pull ruby@sha256:cc089a11b5dfdbaa942fab06c752ea8258d5951786d8e1ccf3df72ef31d7910b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54548786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17d554c39d79da17258abe53fdaa35f33e66cb2984f4e187bcbd1c16faba653`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:34:44 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 07:34:45 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 07:34:45 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 07:38:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:38:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:38:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:38:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:38:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:38:40 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1e54727b8d87779ba8646d7684edc6d5be4ce664280eba37e0634ba03fcb64`  
		Last Modified: Wed, 18 Nov 2020 08:20:44 GMT  
		Size: 22.0 MB (21986385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fc7f20ea70bea6b1d9c326269082b22722fdf90c0725353585183610aabde4`  
		Last Modified: Wed, 18 Nov 2020 08:20:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:15d40531677ec4f2549ce70f96b733981ed1b8f720b384d5db0ce622e73a4cdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59806603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b4fcfafbe48e4e6f3b6c17d875525beba8a2556b8f2fe677d0747725d7c10`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:09:59 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 10:09:59 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 10:10:00 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 10:13:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:13:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:13:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:13:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:13:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:13:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894fdbd265147526c878817f5bd98f8361de57934fa3c8bc1e0daf199a0a4181`  
		Last Modified: Wed, 18 Nov 2020 10:43:49 GMT  
		Size: 22.7 MB (22699036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f40357af6823b101f22af036013f2f75484fcc9f2e1e4514438fd105598251`  
		Last Modified: Wed, 18 Nov 2020 10:43:46 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; 386

```console
$ docker pull ruby@sha256:cee4954d911e0fea0556218206a9371431f771ee4b30c75d690f22ed068b4b24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67274313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d72e7a5f9accbe1c41d509a5acbc598cd74c348c1001adec512907803841ac0`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:01:51 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 02:01:52 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 02:01:52 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 02:07:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:07:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:07:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:07:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:07:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:07:42 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b331efaf53d33cb600b0c212c9ea4184a1acd9977cf72c35632f0c1e1417a2`  
		Last Modified: Wed, 18 Nov 2020 02:50:38 GMT  
		Size: 22.3 MB (22300359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25c36212685d98e8e0b91028052e624eaf79dd16dc5429fbff678a75dfed477`  
		Last Modified: Wed, 18 Nov 2020 02:50:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; mips64le

```console
$ docker pull ruby@sha256:455db03ae9a3855749f806991ddeb7b3c6622f92c6e9e50ef93c125e575fc174
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60458725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fe9583ff9b36d8cb019a6a19a7513ad2007ff3d613b6b73a1231f8ae503350`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:17:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:17:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:17:03 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:35:36 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 10:35:36 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 10:35:37 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 10:44:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:44:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:44:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:44:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:44:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:44:49 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53444f53a30f1399072eca4fd009a136179c00491def98e6d0bd23b1b2155e3`  
		Last Modified: Wed, 18 Nov 2020 11:19:46 GMT  
		Size: 11.6 MB (11607538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa85f0a7be5658739f9f9b8f1038627afc22ce9bac17274b411c4ddf9ba2085`  
		Last Modified: Wed, 18 Nov 2020 11:19:35 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1921eef92e61556065005688bfe3f88d0bc96347824d203351f187ae219cfc`  
		Last Modified: Wed, 18 Nov 2020 11:20:53 GMT  
		Size: 23.1 MB (23073368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a2a480c2c7fef4c166bf7adf1312de47af8aded2451bc98cd01ac9bb05610b`  
		Last Modified: Wed, 18 Nov 2020 11:20:43 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; ppc64le

```console
$ docker pull ruby@sha256:7a0e533b6457e5dfe96c569e98b56c3d82675f17111c70ef8549851e9f39698e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66610227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55871de92e1cfd154ead0353efe1ac659069670163096bad54f57767587e76ef`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:41:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 12:41:19 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 12:41:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 12:50:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 12:51:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 12:51:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 12:51:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 12:51:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 12:51:28 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4def7cf3ccafc158178a77e783d5cbc00b7dc3ba5283bbfd128fbd12ef183b`  
		Last Modified: Wed, 18 Nov 2020 13:23:18 GMT  
		Size: 23.4 MB (23390294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378b4775aeb56bc655ea1a60e3816f19bc39a8bff1063002aa63bd51b1d7b3b3`  
		Last Modified: Wed, 18 Nov 2020 13:23:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim` - linux; s390x

```console
$ docker pull ruby@sha256:7356598c1fabbb47837822a4cf334cb44cf95e9b1eced47435df6d811073aa7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59551531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc669d50856a262ed992f7bdf2de7f649a7de3a899808ca3e1fb7f08bbdd6b8`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 04:28:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 04:28:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 04:28:56 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 04:49:59 GMT
ENV RUBY_MAJOR=2.7
# Wed, 18 Nov 2020 04:50:00 GMT
ENV RUBY_VERSION=2.7.2
# Wed, 18 Nov 2020 04:50:00 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Wed, 18 Nov 2020 04:55:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 04:55:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 04:55:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 04:55:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 04:55:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 04:55:37 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a98fffe2d6da894a31c6905557ec7b9a02fe33b20ba38709b434fa48e23d0a`  
		Last Modified: Wed, 18 Nov 2020 05:37:53 GMT  
		Size: 10.8 MB (10796437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf82c9843c0ec2ead9d4b0d58642fa5d91e80f4cb5bdb641abeb491808dd2ca`  
		Last Modified: Wed, 18 Nov 2020 05:37:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7b79fa47c02023ecc14320c4702276b3486b3689bf08a20a8a70e4b3289a96`  
		Last Modified: Wed, 18 Nov 2020 05:38:24 GMT  
		Size: 23.0 MB (23033577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5c37c13be6f87bdcc071a3fa1c188ac4181f375ae855573584db6e765caa7c`  
		Last Modified: Wed, 18 Nov 2020 05:38:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
