## `ruby:3-slim-bullseye`

```console
$ docker pull ruby@sha256:1fcbddb09232b8c5ca513bf7a099e47a930de31f70db490bfa0c76b9cad68e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ruby:3-slim-bullseye` - linux; amd64

```console
$ docker pull ruby@sha256:ff6a0bac144b82b8ffdad04397e69e4b4515b0d3ea25fb1c47108b50d9148f57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70170610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58692618a3860c4d550076aa955dbb179f3c0bb9d498a5c8edfa9ad8bf8ed06a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:06:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:06:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:06:03 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:06:04 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 04:06:04 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 04:06:04 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 04:10:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:10:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:10:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:10:36 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:10:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:10:38 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4611702bc9d5503ec5b2e69ac04567197afc7acc3de1c10946c3f275e84574bd`  
		Last Modified: Tue, 17 Aug 2021 04:40:35 GMT  
		Size: 10.0 MB (9987127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457bed9fad3b10e3f613b5268ac6fc8d9b4e1fa8bc06bd1ff6f2b43e041c6bef`  
		Last Modified: Tue, 17 Aug 2021 04:40:33 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1033327d29e8ed65f49aaec81abdf2e0406930abf0ae912352f17e760cd2bb5e`  
		Last Modified: Tue, 17 Aug 2021 04:40:36 GMT  
		Size: 28.8 MB (28821796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca57a1697829abe6442a18abd19ce2ab3a15ce3de1ab268c083b295d4009f10`  
		Last Modified: Tue, 17 Aug 2021 04:40:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:0cab55d1d3e25cd587b0d88ae34b5a0d62b56d5bdfe4ab92d249c085d9137f6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67786211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ed01f63cca239beef54646d1239985a83b38d75857d996ef3b1b89eb33bc84`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:08:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:08:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:08:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:08:18 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 04:08:18 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 04:08:18 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 04:10:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:10:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:10:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:10:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:10:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:10:49 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b45cafed299ce7251c1ff6ac6a44cd5c21d6cacfd4f4d57ab85b723e1b5f4c2`  
		Last Modified: Tue, 17 Aug 2021 04:33:35 GMT  
		Size: 9.2 MB (9239497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755e374213bfa2196e6e1f22d096c9494bd306cfddbce4ac6a0d2dbb72a6295e`  
		Last Modified: Tue, 17 Aug 2021 04:33:33 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781ad38c912036aa22849d7947122e533b1e9308e670c18352fd946032c89a45`  
		Last Modified: Tue, 17 Aug 2021 04:33:37 GMT  
		Size: 28.5 MB (28497539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4813697ca1fe11c67ef78cc7324f19597624820091e5a25af2509092a29344d`  
		Last Modified: Tue, 17 Aug 2021 04:33:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-bullseye` - linux; s390x

```console
$ docker pull ruby@sha256:3fbbc3476b3c62179f58bdeb45ffbfe7a40f0c465e5217dbe6fef1de9f12de59
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67468446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56444c949bc1ba87b1e967ab985334ddac708c72b03b393766c8618084c22041`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:17:07 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:17:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:17:09 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 04:17:09 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 04:17:10 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 04:20:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:20:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:20:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:20:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63aea67def9ccff3ba23114bb6d00e78a23de7b70273b765a05cbdf42233a72f`  
		Last Modified: Tue, 17 Aug 2021 05:03:28 GMT  
		Size: 8.9 MB (8855341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ee767ca51c251870e7fea479fa0a4c6dde283dd13adf4733e6caa74ab2a0b7`  
		Last Modified: Tue, 17 Aug 2021 05:03:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1bc150024b29a746586058ed439f3240db17a28b4456f7ca053729b8e1be69`  
		Last Modified: Tue, 17 Aug 2021 05:03:29 GMT  
		Size: 29.0 MB (28965704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18348c5b49145054b7daf787116b70bb7e8c0b1d69e1b5d4bd1354d945863cd`  
		Last Modified: Tue, 17 Aug 2021 05:03:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
