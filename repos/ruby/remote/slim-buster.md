## `ruby:slim-buster`

```console
$ docker pull ruby@sha256:9be76b574748c00835bb574d2fd5354772db38d02bab10d197f8f2c28191aa95
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
$ docker pull ruby@sha256:3b34c167b7d09500b1bccae526652e7c9084b1317a15b0d08a759fdbff6fe184
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71826544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93298008fa7b00ec130b5c738c856b1e4042341cfe822a666a38391ee7a57de9`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:41:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:41:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Jul 2022 13:41:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 13:52:06 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Jul 2022 13:52:06 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Jul 2022 13:52:06 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Jul 2022 13:54:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Jul 2022 13:54:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Jul 2022 13:54:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Jul 2022 13:54:31 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 13:54:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Jul 2022 13:54:32 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29977a4a1ecde26c16d3c4e1b025aed87031476bc7e5ce5275279e4a07662ee6`  
		Last Modified: Tue, 12 Jul 2022 14:14:19 GMT  
		Size: 12.6 MB (12575414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15bba18ce23c4c227cad2dfd1e5070b9c891413a3d88fb6e6f3fe7ae8fd85bb`  
		Last Modified: Tue, 12 Jul 2022 14:14:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590fb01e3e58aeaf9110749476dfebfcc8045d90ee36c311445a69319c38a7dd`  
		Last Modified: Tue, 12 Jul 2022 14:15:51 GMT  
		Size: 32.1 MB (32110906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05751d8fb36227f69365ea0dad2d5b9cc9eff48e42008d6d8e42d8567e0ea699`  
		Last Modified: Tue, 12 Jul 2022 14:15:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:8a76a0caa000798335a851aa36bb13ab256c6c818a15042458fe32aa8b80f5f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.0 MB (65987634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671709b1468ef339ca8b87dfa5ba92feb78b6ae04607dbb3dd3ec5917c28137c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 00:51:40 GMT
ADD file:ae02bb368b4b8ce35a4d250031394d4c6d9e5be3b02168f34922bd87dd2bc726 in / 
# Tue, 12 Jul 2022 00:51:40 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 21:22:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 21:22:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 28 Jul 2022 21:22:04 GMT
ENV LANG=C.UTF-8
# Thu, 28 Jul 2022 22:03:24 GMT
ENV RUBY_MAJOR=3.1
# Thu, 28 Jul 2022 22:03:24 GMT
ENV RUBY_VERSION=3.1.2
# Thu, 28 Jul 2022 22:03:24 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Thu, 28 Jul 2022 22:13:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 28 Jul 2022 22:13:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 28 Jul 2022 22:13:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 28 Jul 2022 22:13:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 22:13:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 28 Jul 2022 22:13:49 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e0c9a5e64041e18deb764eddbdc6c3d20b76797d8c2e2eb4c60d4cba21dc486e`  
		Last Modified: Tue, 12 Jul 2022 01:04:31 GMT  
		Size: 24.9 MB (24889765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c7c572ce65df675f38978ef0608692a092d2d354f616698b084dc954058271`  
		Last Modified: Thu, 28 Jul 2022 23:27:12 GMT  
		Size: 10.4 MB (10356013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ad944d32226a1da8c3badbb7f728ebaef42f8204c1e93cd3845d55388e2e6a`  
		Last Modified: Thu, 28 Jul 2022 23:27:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b857274e23d7202cd69007cb6696c5b84118109d2b1c7a714e329ecb6d6425fb`  
		Last Modified: Thu, 28 Jul 2022 23:29:40 GMT  
		Size: 30.7 MB (30741481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f5e3b8b81c8ab63470ddc131995c065635bafafed50cebb5cce5613a513def`  
		Last Modified: Thu, 28 Jul 2022 23:29:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:1fed2d7cf7ff1e6e563eec0be4498e51b2f34b656110adaf0db1262fe49a60b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63240843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827fbe8eaa62e89733227d36d049f8e4a5fdcfe63bd240c56b6cc8d769186e34`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 01:01:01 GMT
ADD file:973159cf2de6d7890ce8caf5c207ff8c15c19c5b6ea8dff5ff223a1cf75e3f60 in / 
# Tue, 12 Jul 2022 01:01:02 GMT
CMD ["bash"]
# Fri, 29 Jul 2022 20:07:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 20:07:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 29 Jul 2022 20:07:15 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 20:30:56 GMT
ENV RUBY_MAJOR=3.1
# Fri, 29 Jul 2022 20:30:56 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 29 Jul 2022 20:30:56 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 29 Jul 2022 20:34:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 29 Jul 2022 20:34:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 29 Jul 2022 20:34:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 29 Jul 2022 20:34:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2022 20:34:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 29 Jul 2022 20:34:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8031e2dc59e1b5a08ece8056d69de81b33dd5912c374507a775965a83ce367a8`  
		Last Modified: Tue, 12 Jul 2022 01:14:01 GMT  
		Size: 22.7 MB (22748029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0df600b891dd153055f3950af30e4fedab75a3b1d34b3dda26b4e390bd934bc`  
		Last Modified: Fri, 29 Jul 2022 21:29:27 GMT  
		Size: 9.9 MB (9874472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abfe862e506aabae50c9c4286bcd6f7b9860ec0b701e5a5fb6efe84ab1e752f`  
		Last Modified: Fri, 29 Jul 2022 21:29:24 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa6f844a596dd792b53827cf700769880c4c17d46565c2c376575607a151347`  
		Last Modified: Fri, 29 Jul 2022 21:31:56 GMT  
		Size: 30.6 MB (30617967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc9b466712a87aa40e7b46520d8f1ac13439145dbe3bd15524e0b376a03b68a`  
		Last Modified: Fri, 29 Jul 2022 21:31:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:8316109847ce00eb846177e6a3a5c13df3d51dcb9205976199c4003efa73c22c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68548574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c706a5bbc47de238a3cf8fb35c2c89af6891a51c83149521b0d2255bb33715a5`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:02 GMT
ADD file:d6b43ca12a2cc7f73a66ace962f04878f02eab9345172028d77c21d3dc94fe0c in / 
# Tue, 12 Jul 2022 00:41:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:52:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Jul 2022 14:52:53 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 15:02:25 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Jul 2022 15:02:26 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Jul 2022 15:02:27 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Jul 2022 15:04:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Jul 2022 15:04:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Jul 2022 15:04:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Jul 2022 15:04:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 15:04:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Jul 2022 15:04:37 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8bd5501da4f4b37ad7488bd0eafa32d8927de3bf1e32747545810f2ca65429ed`  
		Last Modified: Tue, 12 Jul 2022 00:47:14 GMT  
		Size: 25.9 MB (25914236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b2faed92d152737873f5cbb23a549538c3ffbb14ccbc352303aa5c63c9f1c`  
		Last Modified: Tue, 12 Jul 2022 15:25:02 GMT  
		Size: 11.3 MB (11274696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce73ef3f729d4e0efe5f9870015cd7fa7dea3f200f03cda94f1b1f354841e4`  
		Last Modified: Tue, 12 Jul 2022 15:25:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d860f7af280e86da92db80ca350ac70f8a1ed0353b2a6f730691887e3348cfd`  
		Last Modified: Tue, 12 Jul 2022 15:26:53 GMT  
		Size: 31.4 MB (31359300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda7bba1aee8c4fb8468e716a046db764ef56aeb967871cc81b7ce3fd3c2091e`  
		Last Modified: Tue, 12 Jul 2022 15:26:48 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; 386

```console
$ docker pull ruby@sha256:ae43b42024fad20d2e79fd00905fde7b096d6f7ad0e0f8277de5d6e780c17ff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75777813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc0fce52df5bfad63cf8d1eaf4b705635bfc83e4531cfcdfc3d085935f0f321`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:54 GMT
ADD file:127048950e335136312b4abd45e2f6dbcdbf1641675573278ae97951686fc50a in / 
# Tue, 12 Jul 2022 00:39:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:28:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:28:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 12 Jul 2022 10:28:14 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 10:37:46 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Jul 2022 10:37:46 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Jul 2022 10:37:47 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Jul 2022 10:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Jul 2022 10:39:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Jul 2022 10:39:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Jul 2022 10:39:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 10:39:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Jul 2022 10:39:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3f7bc4b396f6bcb2720b727a14ac5d6a9809a1d7c1a3363baea1fe8d8c6249ff`  
		Last Modified: Tue, 12 Jul 2022 00:46:09 GMT  
		Size: 27.8 MB (27799525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1f2eb5b2c809a7b21f84670202adc12310cafc661d9945ef082e16f365b174`  
		Last Modified: Tue, 12 Jul 2022 11:01:10 GMT  
		Size: 17.2 MB (17233213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc79a3b7f74915dee910cf86b2950d0b56242823e81e307b86710b54fdb68db`  
		Last Modified: Tue, 12 Jul 2022 11:01:07 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a77ca5fb7e3ff59baa6b9db7ad495a5c0f73be969b20b1eaf6ec3da792fa72b`  
		Last Modified: Tue, 12 Jul 2022 11:03:01 GMT  
		Size: 30.7 MB (30744733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f52197f1bddae7d9eddc343106413368882677df84bc3043936f53c009b912e`  
		Last Modified: Tue, 12 Jul 2022 11:02:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:66ef2b12e8d9e396533bcd70907dc6267805ce8dc415fc5b87dbe0fd01dcebb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69330646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d141c800d9ebb783acd658f39f6baba2f913f5be8fb55a70a06de6c0ed852f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 04:42:11 GMT
ADD file:7cc67dd9da4d585d8bdaed90523c7a817bb92aac2bb1f83554f2b46a49e0e392 in / 
# Tue, 12 Jul 2022 04:42:16 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 08:19:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 08:19:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 13 Jul 2022 08:19:20 GMT
ENV LANG=C.UTF-8
# Wed, 13 Jul 2022 09:09:08 GMT
ENV RUBY_MAJOR=3.1
# Wed, 13 Jul 2022 09:09:10 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 13 Jul 2022 09:09:13 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 13 Jul 2022 09:21:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 13 Jul 2022 09:21:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 13 Jul 2022 09:21:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 13 Jul 2022 09:21:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Jul 2022 09:21:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 13 Jul 2022 09:21:57 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:33fe211fd200b2017da34e0864d2aff58d6963435c4b3b7d15083f6860c2fe1e`  
		Last Modified: Tue, 12 Jul 2022 04:53:03 GMT  
		Size: 25.8 MB (25814577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6377896cf25563dc0fd6fb7971ee9866f4d2ddc796669e0ab92025998ebd39`  
		Last Modified: Wed, 13 Jul 2022 10:48:10 GMT  
		Size: 11.6 MB (11635548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f39a16945eccf9f186784712f2ed69a5f6c078c3c9aebfd17a791778040c0f4`  
		Last Modified: Wed, 13 Jul 2022 10:48:00 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1bf9fa87a58fab013bc29d1fe04968b692b90da41932b73e29f7ffb4db9452`  
		Last Modified: Wed, 13 Jul 2022 10:50:23 GMT  
		Size: 31.9 MB (31880180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff079dd55feb61cf310367a0c692ad56ac26b1730b9b7d0f70faba2eb9fd601a`  
		Last Modified: Wed, 13 Jul 2022 10:50:09 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:21d2dbaf773734e4d5c01a93c51ba57cfbac1f1194abff8643262b52457e97b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75569006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37936ce5f97b66bf1bf215159939ce96d2321d73818182c2ef9a30579769804e`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 12 Jul 2022 01:26:17 GMT
ADD file:a6b8aff01d22eb4bfa373d809109de5f0a6a7cf7327f2f711c368ba2ecfcb529 in / 
# Tue, 12 Jul 2022 01:26:25 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 05:24:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 05:24:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 28 Jul 2022 05:24:31 GMT
ENV LANG=C.UTF-8
# Thu, 28 Jul 2022 05:46:17 GMT
ENV RUBY_MAJOR=3.1
# Thu, 28 Jul 2022 05:46:17 GMT
ENV RUBY_VERSION=3.1.2
# Thu, 28 Jul 2022 05:46:18 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Thu, 28 Jul 2022 05:49:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 28 Jul 2022 05:49:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 28 Jul 2022 05:49:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 28 Jul 2022 05:49:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Jul 2022 05:49:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 28 Jul 2022 05:49:52 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:6397b3c9c600936bac0b5fca48461dde424703aa59318fe69c30e207bad2e0b7`  
		Last Modified: Tue, 12 Jul 2022 01:38:08 GMT  
		Size: 30.6 MB (30560087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f78a2a0325715ab6c94a8e7eb87988feb55ee3219dbda11066db6c829011c`  
		Last Modified: Thu, 28 Jul 2022 06:38:57 GMT  
		Size: 12.7 MB (12722020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ff026093ab733aa111eed35076496d6ec9b096c7da066e9ca75f33be39620d`  
		Last Modified: Thu, 28 Jul 2022 06:38:53 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0453f10312832fae3629ee769508f0bf31c3bc46847614d3645e7361cd648f2b`  
		Last Modified: Thu, 28 Jul 2022 06:41:37 GMT  
		Size: 32.3 MB (32286521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872b5397797ff8a2fd61d91f67462385caefd8df2df8ee1efd08545ea7b66087`  
		Last Modified: Thu, 28 Jul 2022 06:41:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-buster` - linux; s390x

```console
$ docker pull ruby@sha256:fb21f288720105284d22c77d7ba8e92aecd7800d30e374896b071d9d45e7359c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68624255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5b30d943ed3634074eb2a6d68e0fb9b9624eb8add252393d4428160348d41f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:56 GMT
ADD file:e455828726a550da92d8fc424a6d7694b6be24a8ca52a6152e2ee89d4f7269d0 in / 
# Tue, 02 Aug 2022 00:42:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:03:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 11:03:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 02 Aug 2022 11:03:22 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 11:12:12 GMT
ENV RUBY_MAJOR=3.1
# Tue, 02 Aug 2022 11:12:12 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 02 Aug 2022 11:12:12 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 02 Aug 2022 11:14:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 02 Aug 2022 11:14:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 02 Aug 2022 11:14:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 02 Aug 2022 11:14:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 11:14:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 02 Aug 2022 11:14:07 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:42614a0fa81c110340e6a5a5db155f27bbb6fa8c1e2421b2c2c5f148ea18f35d`  
		Last Modified: Tue, 02 Aug 2022 00:48:34 GMT  
		Size: 25.8 MB (25758761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691f0736152184b1d9f7eb0f997da97231488c6fd7982b248dfbcacbbe10bc89`  
		Last Modified: Tue, 02 Aug 2022 11:32:57 GMT  
		Size: 10.8 MB (10821329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7acc40c3b4a0a1d44f47ab69b3992b747932168b596c59050c6e88c8cad4d13`  
		Last Modified: Tue, 02 Aug 2022 11:32:55 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8e904382b76775fcd658e887780a69501cc1a9d997a34e2421aec2aec40039`  
		Last Modified: Tue, 02 Aug 2022 11:34:07 GMT  
		Size: 32.0 MB (32043789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3f6d3b2fcb7c12dda63c0c26aa71aa68e3fdbb7388a3ff4556ab228e52b75`  
		Last Modified: Tue, 02 Aug 2022 11:34:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
