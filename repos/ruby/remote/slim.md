## `ruby:slim`

```console
$ docker pull ruby@sha256:ce453efd0e8e85152db4e0fd1e5d0b949ad3688b46f82784550ac9f58ba262d3
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

### `ruby:slim` - linux; amd64

```console
$ docker pull ruby@sha256:cffd6de51a7865c2474588e42a9ab7d0b192b288a6657549eae50719ccfa19cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73322689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e87585c63afb306376697307fd767d814c502bf7334cc733cb4448a113ac48`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Wed, 22 Dec 2021 00:11:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 00:11:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 22 Dec 2021 00:11:36 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 20:23:14 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 20:23:14 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 20:23:14 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 20:26:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 20:26:30 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 20:26:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 20:26:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:26:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:26:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc01ab7c5652550bbf2ece79d7d5e7988bf095b5c2694b45d8b89e327781d167`  
		Last Modified: Wed, 22 Dec 2021 01:11:45 GMT  
		Size: 10.0 MB (9987873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622f415b3531141781fbeb36566e60285480007a62c155d7aea9f1da05b0e12b`  
		Last Modified: Wed, 22 Dec 2021 01:11:43 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34515856594356b8852574e7aa42fbd81f86899aba768c7f7c33e062ac3a9742`  
		Last Modified: Mon, 27 Dec 2021 20:45:02 GMT  
		Size: 32.0 MB (31976815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be0cfac501aaace5444d1785d89fc1bb07225e6b1bee6e68ca6cc2b2b044d1`  
		Last Modified: Mon, 27 Dec 2021 20:44:59 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; arm variant v5

```console
$ docker pull ruby@sha256:03ab918f075a32f4c57239067cb586a65739d64eeb8c8b5f1814582c41a8f58e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68054658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec8fb4a73aeee5398c4fa904c2c923a0661ba78170dd7cd2dca24e333dd60d5`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:31:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 12:31:15 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 19:54:29 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 19:54:29 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 19:54:29 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 19:59:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 19:59:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 19:59:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 19:59:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:00:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:00:00 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c365e76a7805a8d43f975f31bb8b8930dfce6a6cbf62f751736284a024a4e`  
		Last Modified: Tue, 21 Dec 2021 13:49:08 GMT  
		Size: 8.6 MB (8630947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33cb71fe1ced394d30e09ab004fe1100fca48e4d612473a44688af4a36f864d`  
		Last Modified: Tue, 21 Dec 2021 13:49:01 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb7a812c22f03e9e5e4f55776a46eefc6b337e3a874dda89acfb093fbdd3fee`  
		Last Modified: Mon, 27 Dec 2021 20:18:37 GMT  
		Size: 30.5 MB (30523081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd509abb6cd1dff90c78f3a6a9b621e3b08321d173334d6cd3f0e10aa3110f80`  
		Last Modified: Mon, 27 Dec 2021 20:18:23 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; arm variant v7

```console
$ docker pull ruby@sha256:5b732934e4779caab55f4ec81dbd2d5f7b4a28d40ce5c506e0fd0f9000912c81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65092080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd72c3257022676684e89f36ed2db9c0adaf63b6ef86a21bd4d04838d83ed20d`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Wed, 22 Dec 2021 03:38:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 03:38:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 22 Dec 2021 03:38:27 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 20:03:25 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 20:03:25 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 20:03:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 20:08:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 20:08:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 20:08:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 20:08:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:08:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:08:23 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ac60350842a7c32cae335e0d10ed613e9de08d7613beb4c4a1e68008aa5efb`  
		Last Modified: Wed, 22 Dec 2021 04:57:05 GMT  
		Size: 8.1 MB (8140851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011ea9111db2360b5591b19aabc25bb41009a4742d0b16f057a79c5c77a8a71a`  
		Last Modified: Wed, 22 Dec 2021 04:56:58 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e08d1a7dfd9ca8c878a130a98aaac4f3ba24cd1ec1d950f1d0080da46c001b8`  
		Last Modified: Mon, 27 Dec 2021 20:38:40 GMT  
		Size: 30.4 MB (30390039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5151576605130f9d739f79b40505358c4be57775955faea273a45d7cb181a5cc`  
		Last Modified: Mon, 27 Dec 2021 20:38:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:41fe12d28a9c880c0890135a2b65ff843f0fa8db40a9d987ac12d37b4a931ff7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70425407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe3e4f5cf33e0fb4bd5556b2ace9303cf556337b87cfce6437c8e6b9c45897e`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:58:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:58:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 26 Jan 2022 07:58:09 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:58:10 GMT
ENV RUBY_MAJOR=3.1
# Wed, 26 Jan 2022 07:58:11 GMT
ENV RUBY_VERSION=3.1.0
# Wed, 26 Jan 2022 07:58:12 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Wed, 26 Jan 2022 08:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 26 Jan 2022 08:00:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Jan 2022 08:00:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Jan 2022 08:00:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 08:00:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Jan 2022 08:00:20 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fe6c0de23292a962d5603b520a3848e16744950d1d2f13ade18ec7c2d0df17`  
		Last Modified: Wed, 26 Jan 2022 08:32:08 GMT  
		Size: 9.2 MB (9238060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266bdc16cf2cfb4ba48333996360e098fb69470c01bdbe8c70768eeb92343a48`  
		Last Modified: Wed, 26 Jan 2022 08:32:06 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634ca30c187f3ff8dc6a501c56fa51b379a79fcc84f4ad02cf9467357405efe3`  
		Last Modified: Wed, 26 Jan 2022 08:32:10 GMT  
		Size: 31.1 MB (31130231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e174abdd23493eea71c6edf8b83568ea5a6088a5cb4a63a12f7501af983a996`  
		Last Modified: Wed, 26 Jan 2022 08:32:07 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; 386

```console
$ docker pull ruby@sha256:18f07e018a9dc146c1f05cd53a7a02abf27c15402cc3cdc12b904945126d8554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74906104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb9b78fda7b3ddd8724b887420a263183998185e2b8e4081c96ffe7dc46c03`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:56:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:56:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 19:56:26 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 20:44:01 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 20:44:01 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 20:44:02 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 20:47:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 20:47:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 20:47:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 20:47:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:47:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:47:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8c5f1af5a7f5b36f89375f60e51be03d28578ea657521602c68c590d13355b`  
		Last Modified: Tue, 21 Dec 2021 21:12:15 GMT  
		Size: 12.0 MB (11991257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31939b2278d7fb52ae1b1722408ff471767cf04ee162131ac4e89caceb7f9f2c`  
		Last Modified: Tue, 21 Dec 2021 21:12:06 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6a5453afd232d46571fb9a5cf8d9479e49222183f779c4af1962bbfa17882b`  
		Last Modified: Mon, 27 Dec 2021 21:09:29 GMT  
		Size: 30.5 MB (30543621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76975f394af7f6c7114d8c834057b474b346b1039e67c3eda64465ef725d355`  
		Last Modified: Mon, 27 Dec 2021 21:09:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; mips64le

```console
$ docker pull ruby@sha256:33a7b66a577584cc14313f02c78c569b47d0a50aabad3c57866427dca38a8c54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71299296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34aef6ab4f3c28a4986660e303198fd6985873d0af0f215b515361018fc1afa3`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Wed, 22 Dec 2021 19:13:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 19:13:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 22 Dec 2021 19:13:34 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 20:18:13 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 20:18:13 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 20:18:13 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 20:29:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 20:29:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 20:29:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 20:29:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:29:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:29:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcaf36eeb312347c2b92f5b4bc67f4690d9a943ce8021152e4eea3b350d9b4e`  
		Last Modified: Wed, 22 Dec 2021 21:32:52 GMT  
		Size: 9.8 MB (9828674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9fc69c8678bc33d42f99ae329ba1f3a091fce713dc2f000f0d866b054a87fe`  
		Last Modified: Wed, 22 Dec 2021 21:32:43 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb686822ae9f4c82780acc74003d3a2d939f4220d2766028b821a12508a0907a`  
		Last Modified: Mon, 27 Dec 2021 20:53:12 GMT  
		Size: 31.9 MB (31851102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68175c060362affdd1fac47868540ce421791a0c358af665bdd4d03f87b4db46`  
		Last Modified: Mon, 27 Dec 2021 20:52:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; ppc64le

```console
$ docker pull ruby@sha256:e6b3a33d64d9fc4c210d82dfbafe0775f7f4775d47d6a57716011c999afc9953
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77879129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ea2d9c37f40e4dc86baaf6006652745545c62103ef10109ce7c63557f4e23a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 20:05:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 20:05:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 20:05:20 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 20:21:09 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 20:21:11 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 20:21:12 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 20:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 20:26:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 20:26:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 20:26:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 20:26:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 20:26:39 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00709b1b8374e56b30fd137b28d4412caed4652f3043b22b6138bb87175cda2d`  
		Last Modified: Tue, 21 Dec 2021 21:53:47 GMT  
		Size: 10.5 MB (10472320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8667fe949c2ffccbdf9c1e28701270b39d86af0bfbdf2e88528f3d29c5b969`  
		Last Modified: Tue, 21 Dec 2021 21:53:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd535c5f39e24d53938753b8d8573b279e2b68c78a3c64c629aeced3b00b2`  
		Last Modified: Mon, 27 Dec 2021 20:48:22 GMT  
		Size: 32.1 MB (32147441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45e4cc06677ad38623c50ef6aa2bcbd9dca99ca97a7101339fd7f917fdc2de8`  
		Last Modified: Mon, 27 Dec 2021 20:48:18 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim` - linux; s390x

```console
$ docker pull ruby@sha256:dc164a359d613002e91aa1440123534dfc786979727030585a100a5852259767
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70289619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5eac6d4d081ec3a2a5380e8b94f59a80351b812e6edd31756276088ae34835`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:27 GMT
ADD file:c8a482d41bf09dfb6484bf2a6e38535bf0594d26dd6eedd5abde4e3cc811fa6c in / 
# Tue, 21 Dec 2021 01:42:29 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:46:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:46:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 21 Dec 2021 10:46:13 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 19:43:57 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Dec 2021 19:43:57 GMT
ENV RUBY_VERSION=3.1.0
# Mon, 27 Dec 2021 19:43:58 GMT
ENV RUBY_DOWNLOAD_SHA256=1a0e0b69b9b062b6299ff1f6c6d77b66aff3995f63d1d8b8771e7a113ec472e2
# Mon, 27 Dec 2021 19:45:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Dec 2021 19:45:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Dec 2021 19:45:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Dec 2021 19:45:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 19:45:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 27 Dec 2021 19:45:58 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:12562551722a758d23ceea9abcdc2bee737e38c8f62a0f3d3afb2cc2626c28b1`  
		Last Modified: Tue, 21 Dec 2021 01:48:15 GMT  
		Size: 29.6 MB (29641636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45540fecb7ad2998cff650e9fba924affedea1bab03fbb22c703722553ba1ca1`  
		Last Modified: Tue, 21 Dec 2021 11:18:50 GMT  
		Size: 8.9 MB (8855964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409d19884198d33a4513b758c5e01b6bd48367b9f35fed988b3f86cd42a4477`  
		Last Modified: Tue, 21 Dec 2021 11:18:49 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bc200e8a04ca2ef185048654832f1eb4ac119b2021260ed80800bfcdce970c`  
		Last Modified: Mon, 27 Dec 2021 20:00:46 GMT  
		Size: 31.8 MB (31791642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6e693e0eb8682540a81bff45df6648160cf1d9d0549785a7a6b43db83f511`  
		Last Modified: Mon, 27 Dec 2021 20:00:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
