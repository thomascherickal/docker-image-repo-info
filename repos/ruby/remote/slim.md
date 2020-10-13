## `ruby:slim`

```console
$ docker pull ruby@sha256:fa62d7aa86a49677ed30bdbb9ec6b291b9acdce4dbd366cf894f90512042de12
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

### `ruby:slim` - linux; amd64

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

### `ruby:slim` - linux; arm variant v5

```console
$ docker pull ruby@sha256:c7f8b462199f63634315d1870fa4d7ae3b3dc6f674497c2b5936c1a052e74489
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57270845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231296fd42300f23f644b9d9d4b54a316864639c00e559dd1cddae95c5c95d54`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:49:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 08:49:56 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 08:59:22 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 08:59:23 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 08:59:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 09:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 09:03:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 09:03:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 09:03:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 09:03:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 09:03:52 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b190cc26949c645ce201c09b964e6a4588e83d85e65858b95712c87d86aebd`  
		Last Modified: Tue, 13 Oct 2020 09:37:26 GMT  
		Size: 10.3 MB (10327332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d1cb7c2069e37275624f523f9166f9c34b1237b5453ffcd093923141d35d67`  
		Last Modified: Tue, 13 Oct 2020 09:37:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef9be2a61feb3517c6deea11418895a4510f5171bc117f2eb19da0ca419eae`  
		Last Modified: Tue, 13 Oct 2020 09:38:20 GMT  
		Size: 22.1 MB (22107146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c27d9a3942fa4f5bb13e4ced7b88c6ce444ec52eb7d444caa4fd0eb42b7982f`  
		Last Modified: Tue, 13 Oct 2020 09:38:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; arm variant v7

```console
$ docker pull ruby@sha256:0d48d2c0e166e2d17593b8c8520b9a108f9695f0236a89339c8923d143dd7783
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54534422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bd9ff4fb3c0f5fd6120287112e28b33dfc872a8fb2a9d40ba08ffa13005f07`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 14:04:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 14:04:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 14:04:39 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 14:17:35 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 14:17:43 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 14:17:53 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 14:22:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 14:22:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 14:22:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 14:22:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 14:22:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 14:23:05 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05494085cbf95ead5ab2fe5a074ac06b4d89c2b6b8004ca9cee2c798aeba1f4`  
		Last Modified: Tue, 13 Oct 2020 15:25:30 GMT  
		Size: 9.8 MB (9847853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d8df7e8ad03013020a9df686eb1fd48af45cc09ed355e4a3a15abd94b40195`  
		Last Modified: Tue, 13 Oct 2020 15:25:26 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef72f0a922806dbeeffa17a419195d1522e6cf16c3e6cb91153c7063bf16d0cd`  
		Last Modified: Tue, 13 Oct 2020 15:26:32 GMT  
		Size: 22.0 MB (21986342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4362a6c8e4454d48125c820023b60e50d830557ae17fb424ad2dc8572a9354`  
		Last Modified: Tue, 13 Oct 2020 15:26:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:cedf1b6af28515b2ee53b7b499afff4d7b6404000c6a823f53e1fe622cce4cb5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59793479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e0efe08ef1393325b9325c34467481d646cdaf8a1b2e493332d600acf8099d`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:50:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:51:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 10 Sep 2020 18:51:04 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 18:51:11 GMT
ENV RUBY_MAJOR=2.7
# Sat, 03 Oct 2020 00:49:09 GMT
ENV RUBY_VERSION=2.7.2
# Sat, 03 Oct 2020 00:49:09 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Sat, 03 Oct 2020 00:52:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 03 Oct 2020 00:52:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 03 Oct 2020 00:52:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 03 Oct 2020 00:52:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Oct 2020 00:52:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 03 Oct 2020 00:52:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247a9287b017a966d0de690e6f816517ca79a726bf60fc80520737f3e2bbd831`  
		Last Modified: Thu, 10 Sep 2020 19:32:30 GMT  
		Size: 11.2 MB (11244619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8adc8d4d4278c05f1bb052618d8e333a2b28eb246cc8e77d088f526242715`  
		Last Modified: Thu, 10 Sep 2020 19:32:29 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cbf1715386bf2795274a9c70ca5061f77663d30b83d670ea621d0b795d33eb`  
		Last Modified: Sat, 03 Oct 2020 01:02:12 GMT  
		Size: 22.7 MB (22699157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b7d1ab9c515ff0c5a9eb6ab251e7fa69e43fcfed42605541e8ae691546f096`  
		Last Modified: Sat, 03 Oct 2020 01:02:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; 386

```console
$ docker pull ruby@sha256:683713f674616cbbd861e755dcee0eba09d4ed7e43125af02880e965eabf1da3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67258331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:280c9ace9928d8a72697da1497f2e4eed5b0a6d5732f0e296d5285ab04913f27`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 09 Sep 2020 23:40:19 GMT
ADD file:08dc20c9cd727ebf02cac6e4b287c3009274682174aee9222494491cd6c671b8 in / 
# Wed, 09 Sep 2020 23:40:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 15:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 15:44:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 10 Sep 2020 15:44:53 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 15:44:54 GMT
ENV RUBY_MAJOR=2.7
# Sat, 03 Oct 2020 00:47:15 GMT
ENV RUBY_VERSION=2.7.2
# Sat, 03 Oct 2020 00:47:16 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Sat, 03 Oct 2020 00:50:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 03 Oct 2020 00:50:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 03 Oct 2020 00:50:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 03 Oct 2020 00:50:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Oct 2020 00:50:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 03 Oct 2020 00:50:42 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:31e6582dbd9f9a84903d46339df0c393a63d2cbfb001b06b3204653cceafcc61`  
		Last Modified: Wed, 09 Sep 2020 23:46:30 GMT  
		Size: 27.8 MB (27750334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16b111b918a8ba84f9806f6e010b2d15961d77e8c3b1d5c8a4d8f772907d4aa`  
		Last Modified: Thu, 10 Sep 2020 16:23:44 GMT  
		Size: 17.2 MB (17207484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbb541270f5a2ec4b9a8d3ebfc765c744ba546d4c7eedde13fd7b8b70454ea6`  
		Last Modified: Thu, 10 Sep 2020 16:23:37 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908d6d82312fbc75c8f15d797d43db7675078926efbfb7c3338853533ce5078`  
		Last Modified: Sat, 03 Oct 2020 00:59:55 GMT  
		Size: 22.3 MB (22300171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd8cc0503ff778fbb66c0ceba0913d7734da62267f90e4599ca7942f0d1c39`  
		Last Modified: Sat, 03 Oct 2020 00:59:51 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; mips64le

```console
$ docker pull ruby@sha256:530fa718829df2184b40d36c8acd840183092fa1f24eb9588bd7c3c14812b315
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.4 MB (60443604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6726f9a7e7b2e0307525bd15e653c12b9f36483a5d1d7c6bcb0d2b6f11a64f35`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 15:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 15:16:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 15:16:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 15:35:09 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 15:35:09 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 15:35:09 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 15:44:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 15:44:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 15:44:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 15:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 15:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 15:44:22 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e6204b0bc45b22a7266e7a97f2aed1c27ba7598fd69089bd12aa8d40a63af6`  
		Last Modified: Tue, 13 Oct 2020 16:19:09 GMT  
		Size: 11.6 MB (11607653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aecfdf30bae92e5520520ac07c26dcffa1f521a4d5115a56117aa162ce36250`  
		Last Modified: Tue, 13 Oct 2020 16:18:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ee3c1f8da79c69ec61c920985cafaffc38de2886629816f1b1b82b796ccadc`  
		Last Modified: Tue, 13 Oct 2020 16:20:33 GMT  
		Size: 23.1 MB (23073031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf8919dc427fe54bcc3830010aac1ee3afbfb83c20fe7916f7016a6a131c1c7`  
		Last Modified: Tue, 13 Oct 2020 16:20:23 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; ppc64le

```console
$ docker pull ruby@sha256:00b95df71f60def8c6a5eee22c4db4832e9969b26ed3b5deefe508ba12ee1afe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66596457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1bd85923936209411e87273ed1338cbc95bd44ccabf561523c1cb76a42d8ba`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 15:37:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 15:37:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 15:37:45 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 15:50:07 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 15:50:13 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 15:50:20 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 15:58:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 15:59:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 15:59:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 15:59:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 15:59:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 15:59:24 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5a0b847f4c14d1eb300c18d232831f153f16d5db44deb49607211ad4bf05b7`  
		Last Modified: Tue, 13 Oct 2020 16:39:41 GMT  
		Size: 12.7 MB (12687920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae30dfee309351b4a0c588cf263c4cdc35465830372bbe9ad4eb545a0e949901`  
		Last Modified: Tue, 13 Oct 2020 16:39:09 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc995b9a54ccb44a1f70d3a51a11020e7eec483d6fe5b067d732d662aed42796`  
		Last Modified: Tue, 13 Oct 2020 16:41:05 GMT  
		Size: 23.4 MB (23390282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c2bce5cf78a1e52b0de9cc7cef3c1320d45e3a9c8e6196d7ef2f7906c44440`  
		Last Modified: Tue, 13 Oct 2020 16:40:46 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; s390x

```console
$ docker pull ruby@sha256:cb8e78f9683433328cf71700d560c2bbc59973f776bc0cfac16d111bd2360ad7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59538078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57a6315e84f05ff89d31b574d14790d01c217da4b93bf3f9d77df9e33fcd856`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:54:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Oct 2020 05:54:36 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 06:05:39 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Oct 2020 06:05:39 GMT
ENV RUBY_VERSION=2.7.2
# Tue, 13 Oct 2020 06:05:39 GMT
ENV RUBY_DOWNLOAD_SHA256=1b95ab193cc8f5b5e59d2686cb3d5dcf1ddf2a86cb6950e0b4bdaae5040ec0d6
# Tue, 13 Oct 2020 06:08:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Oct 2020 06:08:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Oct 2020 06:08:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Oct 2020 06:08:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 06:08:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Oct 2020 06:08:20 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91453ac8679460a9f899d54654e7e785be8969f76170cbb7f9e67e173554829e`  
		Last Modified: Tue, 13 Oct 2020 06:27:43 GMT  
		Size: 10.8 MB (10796477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d24bb464c8602511abdb6522b8cdb8d5d2e5dc08fe479f571cc41a55b8264e`  
		Last Modified: Tue, 13 Oct 2020 06:27:41 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c56d37b349aae67f7822dbbdaeffbfce9631aeac1fa309bc1133e5d58d4c92`  
		Last Modified: Tue, 13 Oct 2020 06:28:07 GMT  
		Size: 23.0 MB (23033708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1192fc9bc866979b24f78662e049f709c26e63c2f4c008e1b660aac436a65084`  
		Last Modified: Tue, 13 Oct 2020 06:28:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
