## `ruby:2-slim-buster`

```console
$ docker pull ruby@sha256:70ba686baa7958fb0b4d68b8b6b071f61980aa3bb3aab23b094a50e21e6009b0
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

### `ruby:2-slim-buster` - linux; amd64

```console
$ docker pull ruby@sha256:76bfc0d1c091079dbf0964c6c03a466281a231dae11f393463a0bc1e7d3bd6a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54263978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14693b8499376c766d7637c0889db05e1cd1b370fb7118236ce5cf69038825bd`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:53:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:53:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 13:53:29 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 14:19:08 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 14:19:08 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 14:19:08 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 14:20:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 14:20:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 14:20:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 14:20:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 14:20:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 14:20:55 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1deab5c467752dc1ff271d1926326e23b8a5ee00a4ba0498ecc56a5e1487ef`  
		Last Modified: Wed, 20 Apr 2022 14:31:32 GMT  
		Size: 12.6 MB (12575227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ec9d073812451287ed13e111307c9386052b3a1166ff05bcb1b0408d41578b`  
		Last Modified: Wed, 20 Apr 2022 14:31:29 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa353fdaf99ee5763f9801832727516fe0e4d44ec3e882edbedfc7fb28b9ef3`  
		Last Modified: Wed, 20 Apr 2022 14:35:22 GMT  
		Size: 14.5 MB (14547712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c420ce9568ea1d9d0f5f490ef10f4589fdc4d2ee92b483538c162e1b2584637`  
		Last Modified: Wed, 20 Apr 2022 14:35:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:398513ca444ef3febe8d4dca3924e218e6b659755d06f9d0665f59073e3a2ace
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49148468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14f72afa94f7e714b07e139ec58438c3f6fa513bf2d4cea958ed4da450c6fea8`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:47 GMT
ADD file:5b740716d202d2f3494df5e108c0ba999125920ed9c97803fe0ccdfeba5cf518 in / 
# Wed, 20 Apr 2022 07:17:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:22:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 21:22:25 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 22:21:12 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 22:21:12 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 22:21:13 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 22:25:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 22:25:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 22:25:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 22:25:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:25:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 22:25:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1fc8704cfa531d4583c5d4d571b836a82c02a812dae88792c4397cf1c1770405`  
		Last Modified: Wed, 20 Apr 2022 07:33:54 GMT  
		Size: 24.9 MB (24889592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fa4f5186cdac36b883349f2a4c873674b796d97d8205016f21caffcc03559e`  
		Last Modified: Wed, 20 Apr 2022 22:50:57 GMT  
		Size: 10.4 MB (10355807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0d10b4fa5ade38a8ac4858b320fe9a2a7117fd461efe20047339ac801689f9`  
		Last Modified: Wed, 20 Apr 2022 22:50:52 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5720c73f045356aafb738a2b9921b2c7a4619024c6f4fdbcb3e6f21b0e22a8`  
		Last Modified: Wed, 20 Apr 2022 22:56:53 GMT  
		Size: 13.9 MB (13902696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3baee99dc4c87b5880c298392622d22ca470a182016fb9bdff338cdc8531581`  
		Last Modified: Wed, 20 Apr 2022 22:56:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:207310a7bbc51e43fad820b09b80ca58a862d4f629cee1513f575074e5b93b7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46427521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b499828195955b46d75b5a07dda6b7e56de4850b30bb7b287a91942554e4062f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:40 GMT
ADD file:8d54e000817531229c35a32eee074105c7b4d3c08b7ca56b1abdd80571687f28 in / 
# Tue, 29 Mar 2022 02:19:41 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 15:13:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 15:13:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 15:13:30 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 15:51:08 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 20:07:49 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 20:07:50 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 20:11:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 20:11:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 20:11:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 20:11:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 20:11:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 20:11:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d4bf0b27c669e589de33695047d638174fc2ca819a4366d5f80d1ad6b01c0c0e`  
		Last Modified: Tue, 29 Mar 2022 02:35:26 GMT  
		Size: 22.8 MB (22753045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04862a4df372593524d65e6b7c2365699b0398767c88c0fab28bf6a99781d104`  
		Last Modified: Wed, 30 Mar 2022 16:28:04 GMT  
		Size: 9.9 MB (9878660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548be5969b8b14b8d1bcf6dc49c6a130fe52b692a652b5b24817fea6db90f73b`  
		Last Modified: Wed, 30 Mar 2022 16:27:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fcbfe6d78f0487129784a6db45e6902e4e89f71dd2af868868c3a74f7f2715`  
		Last Modified: Tue, 12 Apr 2022 21:03:36 GMT  
		Size: 13.8 MB (13795440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca374ca5f6f297df0b2913af2c5241fd150ed7376e6fdeb76f6c120d0fa03402`  
		Last Modified: Tue, 12 Apr 2022 21:03:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:cdf7e07a5ad685acbc01782da7f2c18e2742b711012d2c6d3a9c55e2c97ba818
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51356933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41cc4ebc9d67d04fefa5dd7ec063aa285c4c47766f66ff59ced0ed5c0970f9f`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:29:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:29:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 12:29:07 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:54:53 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 12:54:54 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 12:54:55 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 12:56:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 12:56:37 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 12:56:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 12:56:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 12:56:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 12:56:41 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77bf0e4ce7a30a322abda93e53b03cb918a055a6ed81e9fd64af6b89ca12f11`  
		Last Modified: Wed, 20 Apr 2022 13:09:31 GMT  
		Size: 11.3 MB (11274388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b549c099b7e79348caf083f065440e3a949b9804c1d7f0d928e46147a6d28a5`  
		Last Modified: Wed, 20 Apr 2022 13:09:29 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2ebb82c16e7bc22aff01b2bfd6289a7ee86a85ff011befc787c81122e6599c`  
		Last Modified: Wed, 20 Apr 2022 13:14:11 GMT  
		Size: 14.2 MB (14173856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2f6bd6e287bec4a9c7572c6f1789d3a1ba762a6ac60b55bc40b8c412090d1f`  
		Last Modified: Wed, 20 Apr 2022 13:14:09 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; 386

```console
$ docker pull ruby@sha256:ff1bc57d7d10298c06822130a76f7df6887d04994ffeac6be69755d6372f01d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58838211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26594d11d1e9932b26aafc3af6aaa00a3993c4187bc5e2c6bf22214ef318f66e`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 07:38:03 GMT
ADD file:602a25173054242f635a5a299845b7f1b56864ac5d3b8af1ae29dec3a9da119f in / 
# Wed, 20 Apr 2022 07:38:04 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 16:29:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:29:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 16:29:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 16:55:50 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 16:55:50 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 16:55:51 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 16:57:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 16:57:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 16:57:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 16:57:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 16:57:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 16:57:35 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a13b13d818745c4d2234aab71df26e4a01bfe59f396ab62f20d156b94803650c`  
		Last Modified: Wed, 20 Apr 2022 07:45:46 GMT  
		Size: 27.8 MB (27799825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8adf63751cdcda285c6be0ce9703ea1d9a81d8a65fe1cc6b43a7aa4ac0d2c16`  
		Last Modified: Wed, 20 Apr 2022 17:11:08 GMT  
		Size: 17.2 MB (17232751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6abfc79ff6d122a3d9fe8305741b72a52a369ba65026a0f7e4b8e3796cbadb`  
		Last Modified: Wed, 20 Apr 2022 17:11:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d38fce7e3e2437fda97cd72a961240de8a909293551476fff07a8e01234eea`  
		Last Modified: Wed, 20 Apr 2022 17:16:08 GMT  
		Size: 13.8 MB (13805293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0f7c1b2c46ec9dd541a62e0e06d05bafb6761f115c62f41396a952324deec1`  
		Last Modified: Wed, 20 Apr 2022 17:16:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:7acdb06e93dfde4e67b9790fba9fd8cba1ba8a1ca032948bce76172114584ea2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51912080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c38693120580023f221cbd02370b5f5d53a1976e109f5181425a9156199d5833`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:36 GMT
ADD file:7827dc4070f09537c063b825b0b7a5b076fac295f9afa415dee6c5346c38d46b in / 
# Tue, 29 Mar 2022 07:43:40 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 23:21:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:21:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 23:21:30 GMT
ENV LANG=C.UTF-8
# Thu, 31 Mar 2022 00:48:07 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 21:11:40 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 21:11:43 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 21:21:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 21:21:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 21:21:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 21:21:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 21:21:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 21:21:40 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:4a3e27ca4ec7041c36d0e9cbc672ce565851ce1a0cc90120d7a923a938fb3c18`  
		Last Modified: Tue, 29 Mar 2022 07:54:19 GMT  
		Size: 25.8 MB (25818066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688c28c235bb0f206cefd09d09e72f759f68d1c40afcc5441389b73d5be28a06`  
		Last Modified: Thu, 31 Mar 2022 01:41:14 GMT  
		Size: 11.6 MB (11640975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b84c61c7467e883a5945955241f7694b03859f7fa8ca53c879889d58d574`  
		Last Modified: Thu, 31 Mar 2022 01:41:04 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cda44718bda10fce2a27aa4f3c537cd13eeea1fd29f973d9824b2a081352624`  
		Last Modified: Tue, 12 Apr 2022 22:08:46 GMT  
		Size: 14.5 MB (14452694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f99c779bb92879e277994a532a4eeeed7d62db1ebf8838816c5d187cc3469d0`  
		Last Modified: Tue, 12 Apr 2022 22:08:39 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:126d75414b3e284e0bc1dcabc864f3a7a6188c3c9374a88afed35f4c2f80d317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58316613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542b95c5751d41cc3d9e0cb3def514eab36baaa0da17026e65f364acb585f1f4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:59 GMT
ADD file:7271d778d432a07f57fedf8d50d83699ef545acc9db9346f6fe75b0054af4cd1 in / 
# Tue, 29 Mar 2022 00:23:00 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 20:23:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 20:23:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 20:23:19 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 21:04:45 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 20:24:37 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 20:24:40 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 20:31:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 20:31:17 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 20:31:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 20:31:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 20:31:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 20:31:30 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:7db831386ce67ac1cf2b4f1513fe3746c9ea2b8d4c82efca75be638eaf533614`  
		Last Modified: Tue, 29 Mar 2022 00:34:41 GMT  
		Size: 30.6 MB (30560163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308b496e1e95a5feaf264a7cc31e6b3c3374fe5e96c73fe9189627bc50dc558`  
		Last Modified: Tue, 29 Mar 2022 21:51:39 GMT  
		Size: 12.7 MB (12724933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2deab05a4a7c0b5c756150a843ec69322aa059b31c6b469fae6c15e5e74aaa25`  
		Last Modified: Tue, 29 Mar 2022 21:51:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367429ac59b848476c26b5708dd60379abff778d84ec98fcf2b5426842f7d0ff`  
		Last Modified: Tue, 12 Apr 2022 21:21:22 GMT  
		Size: 15.0 MB (15031143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d984b4e358df4e6039f0dd80ea62eca90e342f00e4d82926d2e4b7a6937cb5dc`  
		Last Modified: Tue, 12 Apr 2022 21:21:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-slim-buster` - linux; s390x

```console
$ docker pull ruby@sha256:fcc3b160ce6853ad67be9e39018f6e3273a8a576f93e352df430286eb5de78d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51316729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e4f3dd7efffbc8cdf18a53f9ec1ae61a86feb463b296fd82c038457908b094`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:41 GMT
ADD file:e9840ab2ce3aeff61b68bf4837f65471a86dcba02c5023863f3e7493098b07ba in / 
# Wed, 20 Apr 2022 08:40:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 18:18:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 18:18:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 18:18:37 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 18:59:42 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 18:59:42 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 18:59:43 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 19:02:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 19:02:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 19:02:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 19:02:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 19:02:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 19:02:47 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b59fdcf2cb29d2ee4dd08aa08a467372e33525431c4caba9b01e9eb28f76425f`  
		Last Modified: Wed, 20 Apr 2022 08:50:14 GMT  
		Size: 25.8 MB (25758600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9f9c47487b180bf1fddc06918ef1b690d1c893533f21d2767110c45626351f`  
		Last Modified: Wed, 20 Apr 2022 19:21:32 GMT  
		Size: 10.8 MB (10821134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca0be762d292fcd2dc5a0a5b3e49cfd491b26e59df287d2bd8258cfa6f59d35`  
		Last Modified: Wed, 20 Apr 2022 19:21:30 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b081e74980d34a9657c8617d5d8fc9e6ed37a4512e63051bbab0163c1c0d8`  
		Last Modified: Wed, 20 Apr 2022 19:25:24 GMT  
		Size: 14.7 MB (14736620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5254425938aa549f23454c7f26744718f47969bc987b7e97e311fae2c073c361`  
		Last Modified: Wed, 20 Apr 2022 19:25:23 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
