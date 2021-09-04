## `ruby:slim-bullseye`

```console
$ docker pull ruby@sha256:fa3a11fda4d575814308bcbb037bfd3bf4431ae6e009b1105210d5011515279d
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

### `ruby:slim-bullseye` - linux; amd64

```console
$ docker pull ruby@sha256:4a799cc0069603f9a9b6a98c92cd6fc378746f45c4696d09f274b598b5067cf0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70178668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9227622ce12d7e345ab1d41a92ca21ca46d91fafae64fc494b30d487d4a5c011`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 14:07:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 14:07:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 14:07:58 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:07:58 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 14:07:58 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 14:07:59 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 14:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:12:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:12:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:12:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:12:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:12:12 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddf747b7dee00ca5fcb442fe38ba24c54aeb8beb6c80984e8a6f26824e5cc5`  
		Last Modified: Fri, 03 Sep 2021 14:56:51 GMT  
		Size: 10.0 MB (9987613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b86233f7b0e0d092a547cfec1bc67fd7b8c98ba10b648dea0ac0024f9736bd`  
		Last Modified: Fri, 03 Sep 2021 14:56:49 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8facfb3aa184faec4c33b2459fad7f6d566861cee7d96dabc1fc4479dcb67a0f`  
		Last Modified: Fri, 03 Sep 2021 14:56:52 GMT  
		Size: 28.8 MB (28821984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e35af7200cef708c1b46ae3184d31bafa7c354a6d98d44a4cd95a12eea5f5`  
		Last Modified: Fri, 03 Sep 2021 14:56:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; arm variant v5

```console
$ docker pull ruby@sha256:d92def0f31a790329dc07f676d6ad80f908e8ca082545a73194ef3b12c1f9e2c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65372350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:999ecd7742f6e693f2f49e53512a2aedf54ca777de5b1387065fcdfe7c204bf2`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:28 GMT
ADD file:3370827f2aa0dc43cfc2dcb693f82d3f450a70850de7e2514117e366f660d302 in / 
# Fri, 03 Sep 2021 00:50:29 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:03:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:03:12 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:03:12 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 17:03:13 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 17:03:13 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 17:08:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:08:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:08:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:08:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:08:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:08:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:f97b1d091d60e08b0ff779d3cf24a016e55312c03d0930408ff1e1f18d486139`  
		Last Modified: Fri, 03 Sep 2021 01:05:38 GMT  
		Size: 28.9 MB (28910713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7d5ca844b96128489005b10c030be8d299ec60d797d6b814cfa1d08e62dfe9`  
		Last Modified: Fri, 03 Sep 2021 17:58:32 GMT  
		Size: 8.6 MB (8630801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dbe24a80203103ac50302a1df2edb36ff6607e097ca00ca7d36d0829ec7091`  
		Last Modified: Fri, 03 Sep 2021 17:58:25 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c881ba1be60e85fe97224042ff001c4bf6df1dfca1ca93943959c9bf07b2f11e`  
		Last Modified: Fri, 03 Sep 2021 17:58:36 GMT  
		Size: 27.8 MB (27830465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b03640318b98f66d7ed3ad2dd6b61a6b65043f36d3a4df1b44c99f9abd3fcf`  
		Last Modified: Fri, 03 Sep 2021 17:58:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; arm variant v7

```console
$ docker pull ruby@sha256:6cb3c0ba621b2b88f17a6bb4148b3baf725d960be1126a350f06bfc578f3f790
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62422447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ff7ab6339fc16466f8439ab35dd21733be1a3e5a0c2c5b0c70eecf514a25c8c`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:59:39 GMT
ADD file:94917ec8eb06f96483e43104557dd98e5160895900a9d49318eecbb3d5689d41 in / 
# Fri, 03 Sep 2021 00:59:39 GMT
CMD ["bash"]
# Sat, 04 Sep 2021 04:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 04:56:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Sep 2021 04:56:45 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 04:56:46 GMT
ENV RUBY_MAJOR=3.0
# Sat, 04 Sep 2021 04:56:46 GMT
ENV RUBY_VERSION=3.0.2
# Sat, 04 Sep 2021 04:56:47 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Sat, 04 Sep 2021 05:01:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Sep 2021 05:01:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Sep 2021 05:01:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Sep 2021 05:01:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Sep 2021 05:01:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Sep 2021 05:01:25 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:9bd46ffb253d51a8cc84bf034d289b4ca60344ca4446bf38633639b54c7c7ab9`  
		Last Modified: Fri, 03 Sep 2021 01:14:54 GMT  
		Size: 26.6 MB (26571627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a283739dc47dfae11453005ed4880e6581874df9dc83021df6cc3c110c67d42b`  
		Last Modified: Sat, 04 Sep 2021 06:04:43 GMT  
		Size: 8.1 MB (8140646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f21f1144b8b794afe249271c337fd702ea08b1b8298ef03f9e546094c6f59`  
		Last Modified: Sat, 04 Sep 2021 06:04:37 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888d5112725eb21a2ce124902febfa7a4d229d29b3a4609cb80ab19c4370a70b`  
		Last Modified: Sat, 04 Sep 2021 06:04:49 GMT  
		Size: 27.7 MB (27709802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44db3531bcd73d34c5c178cbc146c92caa9893b03421ad83d257762311e13e47`  
		Last Modified: Sat, 04 Sep 2021 06:04:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:23661a5adc3f45f5019a2d7cc04f89e97238791294ca58037744bd33fd5e1dff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67792729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c9563822e82ad7f464bdd0f31c663611ab71d2722492917f22aacc9cb76769`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:33 GMT
ADD file:9600a4686ae105acffa54787a7c81f5252e90023cbcfbe37519150b954110c5c in / 
# Fri, 03 Sep 2021 00:40:34 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:56:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:56:11 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:56:11 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 11:56:11 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 11:56:12 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 11:58:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:58:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:58:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:58:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:58:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:58:45 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1901ca797b5ea06f6a4facc81ad772177fdd833ed4329dc86ef126078633b949`  
		Last Modified: Fri, 03 Sep 2021 00:48:51 GMT  
		Size: 30.1 MB (30055483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698ba2d1e43652351e42e05abde07e46abea416a4716a2e7634880a08517d259`  
		Last Modified: Fri, 03 Sep 2021 12:25:58 GMT  
		Size: 9.2 MB (9239840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cdd8e61807254000863210ab8b2c8cc30f0032f598f4a913b9f876404e8936`  
		Last Modified: Fri, 03 Sep 2021 12:25:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc070fe46ab15bd336e0c450e319bbfb742adc51fd1cb8a8c9ecfb843b9660c`  
		Last Modified: Fri, 03 Sep 2021 12:25:59 GMT  
		Size: 28.5 MB (28497034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bcce0919b426ec798c8b1d8127e4c6d4eafbde8183d366fa1b59806b5b7d01`  
		Last Modified: Fri, 03 Sep 2021 12:25:55 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; 386

```console
$ docker pull ruby@sha256:8c67c40cd07c83590faa3bda174013b5e33b3badb996c882a62b1dc9b97b5dd4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72265053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297acadc5d7874acf9382ebbd55f70de3c9b1e009f01f9608e1d6d8cc9603b69`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:52 GMT
ADD file:dcef0e50863a79295fdbbdad2086d337d6935a220550cb8adaedd7929bd7de63 in / 
# Fri, 03 Sep 2021 00:39:52 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:09:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:09:44 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:09:44 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:09:44 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 11:09:44 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 11:09:45 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 11:15:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:15:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:15:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:15:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:15:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:15:47 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e16e03ac165c3106d1f4265c32840999585f4c4f0e56bd13286caeef08c5be9a`  
		Last Modified: Fri, 03 Sep 2021 00:48:04 GMT  
		Size: 32.4 MB (32379875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f849a8c9970246490f2c4e6debdf6c47993b33eaeebc66b420a52487b0640a9e`  
		Last Modified: Fri, 03 Sep 2021 12:07:20 GMT  
		Size: 12.0 MB (11990952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d215afb6659199e2ef2e61856b9d1e4a80980c63f2beb34b114e47a2c1876102`  
		Last Modified: Fri, 03 Sep 2021 12:07:16 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22757f6f7c0333cbac4550d66c0105f1a7a71559bf855ca5d072fbfa339bf92a`  
		Last Modified: Fri, 03 Sep 2021 12:07:21 GMT  
		Size: 27.9 MB (27893857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177f1b9e64cd47b87320766955ba0c372e003e90a5778cb68b6dd2c8377576b0`  
		Last Modified: Fri, 03 Sep 2021 12:07:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; mips64le

```console
$ docker pull ruby@sha256:91586a7a6ecab1715f4184abf8edc9a29f8236ab52f0179f9e6b2ee84e146cbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.4 MB (68403680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393e685cbe274c4ebd602cc7dc8b598514759d4f345c602c20a13d4f3f69ddff`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:35 GMT
ADD file:4dff23dfe5a1c3cf77be5121c29de84ee66c4d10c85faa65f6122da1bfa13500 in / 
# Tue, 17 Aug 2021 01:11:36 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:54:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:54:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 12:54:38 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 12:54:39 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 12:54:39 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 12:54:39 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 13:05:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 13:05:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 13:05:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 13:05:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 13:05:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 13:05:05 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8375ff99ce3f614d73dc69b03575c7ebf072f4e05da52b0319fc3782d5ebb578`  
		Last Modified: Tue, 17 Aug 2021 01:20:19 GMT  
		Size: 29.6 MB (29619986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f08d5793182fd8d343d92e4f106ceca5ab720e1d42222c02d0a2a1a2931758`  
		Last Modified: Tue, 17 Aug 2021 14:07:04 GMT  
		Size: 9.8 MB (9828407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a517bf4e2f3495f4d9fc8147179cbc05b6b025127295de1bc2003af0f8951ca3`  
		Last Modified: Tue, 17 Aug 2021 14:06:54 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ff1a564b30c2acec3cb2046c95965079b1b52f0d457bde8c68afcc7512cd9f`  
		Last Modified: Tue, 17 Aug 2021 14:07:07 GMT  
		Size: 29.0 MB (28954948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c344f8abcc47f5946d5a5bfbc2b8d82d365ffbc2e2237edc56f214f5a997e981`  
		Last Modified: Tue, 17 Aug 2021 14:06:54 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; ppc64le

```console
$ docker pull ruby@sha256:ba10c7f73c848708dece80e7c847e37df6079ef4ed3ea6be139e4b6002330f2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75014017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1704abbe56ed503d1a5918b973cb445055a1bf6fa4d2a54672c7ab252be8f58a`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:11 GMT
ADD file:71b4f3130e43c12907b826b33d9869308eec40607243a12d904fe47311431db9 in / 
# Fri, 03 Sep 2021 01:23:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 19:21:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 19:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 19:21:34 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 19:21:38 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 19:21:45 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 19:21:50 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 19:32:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 19:32:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 19:33:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 19:33:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 19:33:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 19:33:34 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:be889fbf38c25cf263aa8d8c960d58470da7f841ab3f4949b8a1ac5c4514956c`  
		Last Modified: Fri, 03 Sep 2021 01:36:58 GMT  
		Size: 35.3 MB (35272405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df85c28875d90071198cd189441709e2c3f527d1b58409d90ce303979793460b`  
		Last Modified: Fri, 03 Sep 2021 21:06:41 GMT  
		Size: 10.5 MB (10472159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e67a9efa2ae5b0ca9f03275013ab79e1a926d73911d9a42faf7aae7fdbabce`  
		Last Modified: Fri, 03 Sep 2021 21:06:38 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47872e700f606f4872077378a59637f037ce79c3329b298f7c60ef5cfa47d190`  
		Last Modified: Fri, 03 Sep 2021 21:06:43 GMT  
		Size: 29.3 MB (29269083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b59629acff8d77d87924dbf9d0e97554870c299aced5c126b2c02274b8d382`  
		Last Modified: Fri, 03 Sep 2021 21:06:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:slim-bullseye` - linux; s390x

```console
$ docker pull ruby@sha256:f051f7b09addf2adb25c531ff538b18d255d02f75167b1f2381b46add7df915e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67472598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58f818d82caff090845f5e8113450ffea30139e1e8c9ae5df853b07188be074`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:48 GMT
ADD file:9e72d98b2c920e433c6b776ed8eaf6a90cbf367d0ee37a8461d191499be72d39 in / 
# Fri, 03 Sep 2021 00:43:52 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:01:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:01:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:01:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:01:18 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 13:01:19 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 13:01:19 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 13:05:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:05:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:05:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:05:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:05:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:05:58 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:33fe066e16e87fca4bcb280b7ec53d44c561299928e592068e985314cf93215b`  
		Last Modified: Fri, 03 Sep 2021 00:52:58 GMT  
		Size: 29.7 MB (29650625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a3ee02b4e8f64cf827e753c2caec8527967d2bb2e3d16dc57498160ad5b13e`  
		Last Modified: Fri, 03 Sep 2021 14:12:30 GMT  
		Size: 8.9 MB (8855862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bff71a8a32ddfb1a0e1fb13b03e114fa09ee52df98a21820670d98dba5e2aa7`  
		Last Modified: Fri, 03 Sep 2021 14:12:28 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fce2825717425ad21346d08c8890b94a9554ecfee6d282980a572cd87d423a`  
		Last Modified: Fri, 03 Sep 2021 14:12:31 GMT  
		Size: 29.0 MB (28965740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918582b48269001c517211f33182db1a7bd5b57f3ec45234d8a1163fb2e6426d`  
		Last Modified: Fri, 03 Sep 2021 14:12:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
