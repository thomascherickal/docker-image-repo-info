## `ruby:slim-buster`

```console
$ docker pull ruby@sha256:be09419183e31fc3f505fad57305d202e09ddfe25430f22d9071f1e52aad0325
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

### `ruby:slim-buster` - linux; amd64

```console
$ docker pull ruby@sha256:1b0ad1461bd10afc0023b4123b1cd138b695203175384bff11a8e5eb07e0903b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68439759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2102d9e8e004fdf9015d957de0efbb2f5dfa349effa4103d7ddc4ff70641baff`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:33:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:34:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 02 Dec 2021 16:34:00 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 16:53:37 GMT
ENV RUBY_MAJOR=3.0
# Thu, 02 Dec 2021 16:53:38 GMT
ENV RUBY_VERSION=3.0.3
# Thu, 02 Dec 2021 16:53:38 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Thu, 02 Dec 2021 16:58:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 02 Dec 2021 16:58:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 02 Dec 2021 16:58:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 02 Dec 2021 16:58:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 16:58:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 02 Dec 2021 16:58:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90624b6090464f48417857b7235f0e54f5ee684d286beb9fbae0d710e785ad9d`  
		Last Modified: Thu, 02 Dec 2021 17:31:27 GMT  
		Size: 12.6 MB (12565241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e61194650215f6a06f21d197f04bd7bd30adcfec50d4a440007d025f5ce5a00`  
		Last Modified: Thu, 02 Dec 2021 17:31:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dafd5e27377531e152fcc220ed47250a8f332e9cb801f3e0f3900c0830c3df1`  
		Last Modified: Thu, 02 Dec 2021 17:33:15 GMT  
		Size: 28.7 MB (28720414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b621b4afc6c61e0f4728db341418e937b01b8b078893cabe56881b1eef6292e`  
		Last Modified: Thu, 02 Dec 2021 17:33:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:a2cafd7f45839273ecdd6e0372294ffc0a082c288e69008c758e958be9870004
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (63018519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5065581fecdcfbd4e9bbbd123e2954c2ee7360b1bf336cfa54dfa4d670aa8ddc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:32 GMT
ADD file:f757929225218280f26d0eca53387788343e93cc9658f5baeb58957776114579 in / 
# Tue, 21 Dec 2021 01:51:33 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:41:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:42:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 12:42:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 13:02:08 GMT
ENV RUBY_MAJOR=3.0
# Tue, 21 Dec 2021 13:02:08 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 21 Dec 2021 13:02:08 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 21 Dec 2021 13:07:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 13:07:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 13:07:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 13:07:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 13:07:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 13:07:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:7d69cd3acec6d9e5ca88bdd718b069a7272b722048f49b6d21fbe85fc6c82560`  
		Last Modified: Tue, 21 Dec 2021 02:07:21 GMT  
		Size: 24.9 MB (24886253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92df2c99558917fbcf7105700ca98019f713c9592c86279d061d0e3e36e04de8`  
		Last Modified: Tue, 21 Dec 2021 13:50:09 GMT  
		Size: 10.3 MB (10349290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2a4850cb5a6c935604fddab8cfe0ef79d8c356cc290bf3afcad83396ed276`  
		Last Modified: Tue, 21 Dec 2021 13:50:01 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceb2114f5629da654e5027abae5336805ce98dabefa007e19ff02703c558e24`  
		Last Modified: Tue, 21 Dec 2021 13:52:48 GMT  
		Size: 27.8 MB (27782600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823d2fcea26d477e36c6a10f3af0c075f27ee01980da6866686008a08dcd3e90`  
		Last Modified: Tue, 21 Dec 2021 13:52:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:9d965261fd2b8aaf6f3e896493d0f41fc6f6e0c9fe36cb94871684feabd3a32a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60302238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae7dd33a028ddd020e3661e46b34f8444d3d2c34bfb4a025f862afb5c3048df`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:21 GMT
ADD file:7b30d743b30e84b21888f23cb7f266caba09db98b7a4c8800abebcf03d28c01d in / 
# Thu, 02 Dec 2021 09:06:22 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 17:30:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 17:30:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 17:30:54 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 17:50:37 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Dec 2021 17:50:38 GMT
ENV RUBY_VERSION=3.0.3
# Fri, 03 Dec 2021 17:50:38 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Fri, 03 Dec 2021 17:55:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 17:55:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 17:55:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 17:55:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 17:55:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 17:55:25 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2aa85085c98821a25a3058f7fc2c6427064f2228ea8eac904e9e7db4dbdaa01a`  
		Last Modified: Thu, 02 Dec 2021 09:22:26 GMT  
		Size: 22.8 MB (22754365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1787793a37de8674853036139b8cf3e6e54fd257e9b3ab8bba1175936ee679a1`  
		Last Modified: Fri, 03 Dec 2021 18:39:48 GMT  
		Size: 9.9 MB (9872859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db8fa492ac8e0b37299aa54782addae92722be6c2556d52ea0cac13628daf48`  
		Last Modified: Fri, 03 Dec 2021 18:39:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd86f0929c990f24475afd87aafe7f00ffec93bfaa6edc9f04ea57d29a0156b`  
		Last Modified: Fri, 03 Dec 2021 18:43:27 GMT  
		Size: 27.7 MB (27674639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619dc6c22282b7bb6ee39d548be5702b4a692b22148ddbe44ed94f78a9e71dc`  
		Last Modified: Fri, 03 Dec 2021 18:43:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:032ac587849b160b25a58f542662c3ff7a52b22d0181718e46ca6fe9f08f2fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65424534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43b6e76610228d3bcec2fac81b209b45b576f112b32eee3e1aaf5b13c6381974`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:46:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 13:46:11 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 13:54:46 GMT
ENV RUBY_MAJOR=3.0
# Tue, 21 Dec 2021 13:54:47 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 21 Dec 2021 13:54:48 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 21 Dec 2021 13:56:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 13:56:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 13:56:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 13:56:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 13:56:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 13:56:47 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df957e92572da886c36ceee88919e1780eaacc4ffe81dba01dadcc234d3b4636`  
		Last Modified: Tue, 21 Dec 2021 14:16:30 GMT  
		Size: 11.3 MB (11261786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f498124153b35570162f92f7962aa50fd000b9fb69e0789e5e1127c014cca38`  
		Last Modified: Tue, 21 Dec 2021 14:16:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f7acccd73def61929e74331d8689aa67b151dbdfae7968cbbdc2d219612a5a`  
		Last Modified: Tue, 21 Dec 2021 14:18:16 GMT  
		Size: 28.2 MB (28239257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d5b1641f32fe76f2523616ffb24624253ab836f20e056708fe0f59a6cc13c`  
		Last Modified: Tue, 21 Dec 2021 14:18:13 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; 386

```console
$ docker pull ruby@sha256:53054cc56dc1c50dcf670b8630d5b4cb4bd5d5e4be1096b4c20cfde592edd4ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73019693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce2446f3d7e72f6fb55da4dce10a850e34350d6c8fa8c751018ffc23fc3dafcb`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 20:07:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 20:07:40 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 20:07:41 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 20:28:37 GMT
ENV RUBY_MAJOR=3.0
# Tue, 21 Dec 2021 20:28:37 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 21 Dec 2021 20:28:37 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 21 Dec 2021 20:33:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 20:33:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 20:33:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 20:33:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:33:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 20:33:41 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1066d2070153fbad5494fe979ad171707d9eab3b32f3fd90979531049d8b27`  
		Last Modified: Tue, 21 Dec 2021 21:13:06 GMT  
		Size: 17.2 MB (17227036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157ccdbc4b0d00d4ffd83478d4385983d9d4f8c22959750d2de032fa02a762d`  
		Last Modified: Tue, 21 Dec 2021 21:12:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf87ecd8a03d0e06405c0fea4ab4eaff75080bfcbef98d77e62d611416aab63b`  
		Last Modified: Tue, 21 Dec 2021 21:15:17 GMT  
		Size: 28.0 MB (27987708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a31b0fd410985515bead44ff38eaac82c68475e5a43983da4f1cd4f2cf56ff`  
		Last Modified: Tue, 21 Dec 2021 21:15:09 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:875edd2e1aa35dba5e13ed67054b21b2e57901eb38de88b5523bfcf4556bf93b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66367392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8007325fab1046ddbafb7fcfffdd0fc6f789fee1c9de1fb32e18a32628666b3`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 02 Dec 2021 03:10:02 GMT
ADD file:8c95ae1f84ca959b3714f55dc11bf2655dbe383f4aa06564e3f0f5386a8602b9 in / 
# Thu, 02 Dec 2021 03:10:03 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:56:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Dec 2021 01:56:00 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 02:36:12 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Dec 2021 02:36:13 GMT
ENV RUBY_VERSION=3.0.3
# Fri, 03 Dec 2021 02:36:13 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Fri, 03 Dec 2021 02:46:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Dec 2021 02:46:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Dec 2021 02:46:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Dec 2021 02:46:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 02:46:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Dec 2021 02:46:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d19557eca39adc90542589f749291953b676e4201aa77d093caf4a98b87fb79b`  
		Last Modified: Thu, 02 Dec 2021 03:19:22 GMT  
		Size: 25.8 MB (25820168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68590ad0e6ea499fa2cce7ea1cbbb50e068fb8ace83cafd97940264e31728f42`  
		Last Modified: Fri, 03 Dec 2021 03:55:04 GMT  
		Size: 11.6 MB (11629969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d47ff31a2a6d15dcd12ee66d314caad8a67669f3140c8134f858a45396e6c7a`  
		Last Modified: Fri, 03 Dec 2021 03:54:53 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bd0e9d9067f2176e152e92a6b29db4b6379917e519441283ef4f48ff48eb01`  
		Last Modified: Fri, 03 Dec 2021 04:11:29 GMT  
		Size: 28.9 MB (28916913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e680421a6215baae03df5d4ebdeb6b7b35773a257415c607b8e4a000f09b6`  
		Last Modified: Fri, 03 Dec 2021 04:11:17 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:afd9df5166601a0fce9bb0e5eb57e1fd2c58a8cdb6f19b0c11401bacc1cdbdb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72419871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26eaa7dca178942529e52d901bb5ed4cfe15d8cc5620065849cec2b4b50205e0`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 20:19:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 20:20:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 20:20:03 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 20:47:10 GMT
ENV RUBY_MAJOR=3.0
# Tue, 21 Dec 2021 20:47:13 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 21 Dec 2021 20:47:15 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 21 Dec 2021 20:56:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 20:56:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 20:56:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 20:56:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:56:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 20:56:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2631c00b3c311045cc73612901f9f9c688c51a4fddcf564b71e07e86d63a947c`  
		Last Modified: Tue, 21 Dec 2021 21:54:28 GMT  
		Size: 12.7 MB (12705564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fac6323fc58a5c06a4515158cc75b1af10e0f49be49230d25dc2c26ffacd771`  
		Last Modified: Tue, 21 Dec 2021 21:54:25 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aa876fda4a430d38fb4f2dce1555e4e8230959ac798c2845714c99dab9a4df`  
		Last Modified: Tue, 21 Dec 2021 21:56:25 GMT  
		Size: 29.2 MB (29151620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01091a94d976a4bd260cd233bd5ea9ed88ec3dd7b8ffaacf190e4a7f1a774e64`  
		Last Modified: Tue, 21 Dec 2021 21:56:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; s390x

```console
$ docker pull ruby@sha256:ce71b01b9b2c9d266f74f72f6fce546c50f3a4a41df4fd99ef50c62cc3789cae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65498745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcde114e088e5f7c65be457d9ad71b4bc30286c0ae1dd5d104bb4a73e01500d7`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:57 GMT
ADD file:33e37861eefa46f6e5f7f4967ce8ae3167e28bc817c3c71ff90a3d51e2376a0f in / 
# Tue, 21 Dec 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:50:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:50:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 10:50:51 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 10:59:26 GMT
ENV RUBY_MAJOR=3.0
# Tue, 21 Dec 2021 10:59:26 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 21 Dec 2021 10:59:27 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 21 Dec 2021 11:01:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 21 Dec 2021 11:01:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 21 Dec 2021 11:01:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 21 Dec 2021 11:01:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 11:01:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 21 Dec 2021 11:01:22 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:10979941d091693f28e3dc033cc6ca88996acf42a0aace27ad85fbd894945e20`  
		Last Modified: Tue, 21 Dec 2021 01:48:51 GMT  
		Size: 25.8 MB (25769051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a6f3c4642cf35166efc3bc51ae42418989834c8eca28809948ada296bb9c5`  
		Last Modified: Tue, 21 Dec 2021 11:19:14 GMT  
		Size: 10.8 MB (10815241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c51d7f208d075afa3e35cffb33a4058bc2e6b09617649fda7a7cd8522e52308`  
		Last Modified: Tue, 21 Dec 2021 11:19:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b544419a3e40a97cc2a4a962b603b73e45bb9404307dce464daeb23ab4af54e`  
		Last Modified: Tue, 21 Dec 2021 11:20:22 GMT  
		Size: 28.9 MB (28914077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79376544aa778b7888582a0d81d08b9c4da32cc49f720cb1b09966b8ebe14bca`  
		Last Modified: Tue, 21 Dec 2021 11:20:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
