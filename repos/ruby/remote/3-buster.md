## `ruby:3-buster`

```console
$ docker pull ruby@sha256:86f5dc946380ba8794a5d6f71270e25792931824ee4d687d0479b8a89f3a22bd
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

### `ruby:3-buster` - linux; amd64

```console
$ docker pull ruby@sha256:25165e0403e0189a00486df5d6d1b89c319056f3387a195c557c2d7d3fb537c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.9 MB (340946899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0439568f9b50ce4bac28776820f7d1b8d10de15475e4c7431637aeb2f117121d`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:52 GMT
ADD file:b9e6354f7b545096b6cb6072a50de0dffa2232f22d1972a4679f46a7e6394cae in / 
# Tue, 17 Aug 2021 01:23:53 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:20:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:21:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 17:36:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 17:36:02 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 17:36:02 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 17:36:02 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 17:36:02 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 17:38:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 17:38:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 17:38:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 17:38:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 17:38:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 17:38:57 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1cfaf5c6f756207bc4607d40ddd440bd2bfa7ab455b2c3015ccf56d85cd1377b`  
		Last Modified: Tue, 17 Aug 2021 01:29:55 GMT  
		Size: 50.4 MB (50436201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4099a935a96edef1e9378de34e314d07fb3aea1b7205774055a1fa44a3819f4`  
		Last Modified: Tue, 17 Aug 2021 09:30:37 GMT  
		Size: 7.8 MB (7833079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e2960d83651b1494b4da6c97686e79cc760aa90a75948eed56786726f86928`  
		Last Modified: Tue, 17 Aug 2021 09:30:38 GMT  
		Size: 10.0 MB (9997209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd4e6385927b79e4d4daa2d00523e766502eed6dd1934e1eda583d348abd8b`  
		Last Modified: Tue, 17 Aug 2021 09:30:58 GMT  
		Size: 51.8 MB (51841042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce46ad6f244a871abfead80f28a613b68fba68e165467d817e09453b369252f`  
		Last Modified: Tue, 17 Aug 2021 09:31:38 GMT  
		Size: 192.4 MB (192393994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8f4da6b2c89d757bec1bad6014fb6ca2cf208cee58142e23d4770105f18459`  
		Last Modified: Tue, 17 Aug 2021 17:51:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c076facdc402bed746bcffa6b8ff260aae106851193d036ce57b9151eb06da3a`  
		Last Modified: Tue, 17 Aug 2021 17:51:58 GMT  
		Size: 28.4 MB (28445001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993eefd79ddb1b9b866bc5a4a0f3f9f622c5f05c0ba42df38347c8beb04a323f`  
		Last Modified: Tue, 17 Aug 2021 17:51:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:12bccf584c1cbdd0051b5e3e18cbd385fcc74d05048f9c5fe955e50d87810d4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.7 MB (313663204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e40adf820e0b7c9773a43c5f1fc3008315785c16820e403e375902208b2ff057`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:56:17 GMT
ADD file:784cabdb8b1e35aff6dcfa7acb3c6da5d76ee575188460537a190bab6ef49655 in / 
# Tue, 17 Aug 2021 01:56:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:22:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:22:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 09:23:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:25:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:54:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 21:54:44 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 21:54:45 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 21:54:46 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 21:54:46 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 21:59:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 21:59:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 21:59:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 21:59:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 21:59:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 21:59:55 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ce5dcedb6ed028586f61d36e8067567349cb049735f9b1fbeb748a005636b9d9`  
		Last Modified: Tue, 17 Aug 2021 02:11:57 GMT  
		Size: 48.2 MB (48153800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1036818934ab73ac9c3e731432ae2c2c576a342f8ac27c0de1654407945f2b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 7.4 MB (7376657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33acf22e716d76b46aa215be86d402b346c30583ac243161d878e673e2e55f3b`  
		Last Modified: Tue, 17 Aug 2021 09:40:04 GMT  
		Size: 9.7 MB (9687540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824ed8f5821cf4dcfd3bd99d56b7aa9c5eae5312be30686e88b07808d8c0cdc`  
		Last Modified: Tue, 17 Aug 2021 09:40:52 GMT  
		Size: 49.6 MB (49574573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e758f7a7e0da372de0f1611d7468674233f2987fcd71261075cd789d9e68c376`  
		Last Modified: Tue, 17 Aug 2021 09:42:43 GMT  
		Size: 171.3 MB (171327019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace7bedec45135981eb52ac037a232e777efa99bdae5bbdbb390f7c2d9b00`  
		Last Modified: Tue, 17 Aug 2021 22:24:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5933fb63072d10078d0347c6c4efc824f0d7be65f3813a2baf24de2477c4eed5`  
		Last Modified: Tue, 17 Aug 2021 22:25:04 GMT  
		Size: 27.5 MB (27543240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab281b89439891ff09077e6a22b05bd4deb6990d3fcc507a8e73ad0396966af8`  
		Last Modified: Tue, 17 Aug 2021 22:24:52 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:fbb41c086bf19b0fe4a631c04ca8d62433f4d8a477ffaacb029ffc84f481960f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305784245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0a8e9511c9e60f09fe8146a2d31a5e97f18e1be0ac71dfee1ba9aea6e482f1a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 02:13:48 GMT
ADD file:335c38ff88b5e08b7ac0de8108215837affe91919978ea400e32196f7601b991 in / 
# Tue, 17 Aug 2021 02:13:49 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:21:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:24:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:35:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Aug 2021 07:35:32 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 07:35:32 GMT
ENV RUBY_MAJOR=3.0
# Wed, 18 Aug 2021 07:35:33 GMT
ENV RUBY_VERSION=3.0.2
# Wed, 18 Aug 2021 07:35:33 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Wed, 18 Aug 2021 07:39:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Aug 2021 07:39:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Aug 2021 07:39:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Aug 2021 07:39:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 07:39:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Aug 2021 07:39:42 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:978724337d55541757ceda31b51cc0dcbdb70d7d5bc63ebcc0aaceab90aa8acf`  
		Last Modified: Tue, 17 Aug 2021 02:30:16 GMT  
		Size: 45.9 MB (45917818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f0b0065a7e3b0a78d7b7e0691152e1474bfd7bc177bb8a2383c8b14b0c9dab`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 7.1 MB (7124489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6ed7bdd30c985279190b4c2a50b4257a03d5706663e8ec8c766f425014c39c`  
		Last Modified: Tue, 17 Aug 2021 15:41:09 GMT  
		Size: 9.3 MB (9343798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54854fad8c30eacd3b5b5484549685dbf93460ecf31ea30835ec3aa3e3cfa49`  
		Last Modified: Tue, 17 Aug 2021 15:41:54 GMT  
		Size: 47.4 MB (47357324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c39822934191a8ed942f48d7d0005d1f051e099931a35baf8688726dc3ec632`  
		Last Modified: Tue, 17 Aug 2021 15:43:40 GMT  
		Size: 168.6 MB (168592913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac17021bdbb81b88f3da43cf4a013182c992a12be3da32b3891e4b7ee2cf5f7f`  
		Last Modified: Wed, 18 Aug 2021 08:16:23 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6406d4d43eb4728032be4459ec9d73389941cc3cbfe9dbfbe61dec2d1cca2a9e`  
		Last Modified: Wed, 18 Aug 2021 08:16:35 GMT  
		Size: 27.4 MB (27447526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb812f8f3ecf6862285ea85155e04ca274135f63eaf7fa012ef340e357233f7`  
		Last Modified: Wed, 18 Aug 2021 08:16:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:beae85fe28dbd5847e93d8628f6aeced957cbb0bb81f3c7cdfa2f30c19e9c0b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331239184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56e23aaaef6b4bb8b0f02ca989ff329e50b028251a5ce628ec780d38cb62fbb`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:44 GMT
ADD file:1d6e5f5349752ab5c5888d38637821d2943472188c06bd14ea2bdf7a676ea19b in / 
# Fri, 03 Sep 2021 00:40:44 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:33:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 04:34:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:34:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:59:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:59:01 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:59:02 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 11:59:02 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 11:59:02 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 12:01:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:01:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:01:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:01:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:01:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:01:17 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e3c1991bf0816d8624d8191a43732b869478319ed39c5f218e5878ed1ee05d58`  
		Last Modified: Fri, 03 Sep 2021 00:49:16 GMT  
		Size: 49.2 MB (49222144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529bf6c2a9fdb0edf93a87f6fbc959069a0068fe2ed046af546fca48e8ed6ffe`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 7.7 MB (7695770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9703bfb802a7157134df39897b2625906f8057c03e52daa3e8298ca41dfd7b`  
		Last Modified: Fri, 03 Sep 2021 04:42:18 GMT  
		Size: 10.0 MB (9984267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a64745ecb3a1d83570e6c503995c0eb3f97176e23bd91210bf235e5646a4e96`  
		Last Modified: Fri, 03 Sep 2021 04:42:38 GMT  
		Size: 52.2 MB (52167858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a277fe22c4aa02638e00e9df995f81fc80e44710768e66b1067d15d6ebfb117d`  
		Last Modified: Fri, 03 Sep 2021 04:43:16 GMT  
		Size: 184.0 MB (183974353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea5f1e4cb80cad50a4fe8f41b2740c1e3c8b8012dde9f5cbdb7ef18d95b5162`  
		Last Modified: Fri, 03 Sep 2021 12:26:30 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c824145e706f2e7d5dbf8d5ede0a4c2ab02fcf70de111bb34333b27e0b19bc4`  
		Last Modified: Fri, 03 Sep 2021 12:26:33 GMT  
		Size: 28.2 MB (28194423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67453823ef2da07783c10aec95cf3ac791f75d3644cc1af6a9bd76a100fc517f`  
		Last Modified: Fri, 03 Sep 2021 12:26:30 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; 386

```console
$ docker pull ruby@sha256:03cda149246b6f7740b876f5e911c053d657b2dd41319c457962e3f4f8d0bd20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.6 MB (349634627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a549399a177b757521fc696eb9c86c883344c92947cb9b30d3bb88390f1d250b`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:07 GMT
ADD file:b57b08af647bb21d95dcfaaf631569421b159ccb57981aa968957e83d0d88be1 in / 
# Fri, 03 Sep 2021 00:40:07 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:12:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:12:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 01:13:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:14:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:15:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:15:59 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:15:59 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 11:15:59 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 11:15:59 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 11:20:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:20:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:20:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:20:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:20:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:20:39 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:51869ffe8843ba6b44f606117326ad744bef79bc74f8eb46ebdc19e9299ede76`  
		Last Modified: Fri, 03 Sep 2021 00:48:31 GMT  
		Size: 51.2 MB (51207209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8b7c65ab186ac667e4c325c9bc0aedb35fa5c3c0e94bcf31756f2242bad69c`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 8.0 MB (7999823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e5b243d4918f63b95623e21cd2da926e7a519a11f79d5dccbe9e1c921fdb3`  
		Last Modified: Fri, 03 Sep 2021 01:21:23 GMT  
		Size: 10.3 MB (10339942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ad561c8654d0087f55d8ba8f2c88f6bf9760d1a07c98c20226182dd661df18`  
		Last Modified: Fri, 03 Sep 2021 01:21:49 GMT  
		Size: 53.4 MB (53438188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7076e49e31f46f892cc53ebc742d6b7aac932b484254aa2eebc010ca0de90549`  
		Last Modified: Fri, 03 Sep 2021 01:22:43 GMT  
		Size: 198.9 MB (198931128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d88a17a289283d6a46ce790e170dc2e06ded4babe07b0343c61e8b57e5d8ab1`  
		Last Modified: Fri, 03 Sep 2021 12:07:57 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d0cb1a81463a6d23c7caf79437b62a79f8c297093d9af92fcd54397022b34d`  
		Last Modified: Fri, 03 Sep 2021 12:08:03 GMT  
		Size: 27.7 MB (27717966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da68eef6f75bce6f574b0d4b25cbda97a1c32ebad8c769f4a233ce3f3cc271a`  
		Last Modified: Fri, 03 Sep 2021 12:07:56 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:db16e5f663b68ca403cfe8f60300edfd2630739917a108637c084329e7aeb856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.8 MB (325768419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1edea4e25631c63debd3065474bc51e489f49bf0135ef7e16550b0fa7f579558`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:02 GMT
ADD file:a8c2c0d0623fc8523c52507da1bb3e33e40086f0387a0ec12df9480599a1799e in / 
# Tue, 17 Aug 2021 01:12:03 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 20:45:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 20:46:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:49:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 12:02:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Aug 2021 12:02:11 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 12:02:11 GMT
ENV RUBY_MAJOR=3.0
# Wed, 18 Aug 2021 12:02:12 GMT
ENV RUBY_VERSION=3.0.2
# Wed, 18 Aug 2021 12:02:12 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Wed, 18 Aug 2021 12:11:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Aug 2021 12:11:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Aug 2021 12:11:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Aug 2021 12:11:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 12:11:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Aug 2021 12:11:22 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e36b8e9dc7a490231e9a4577c7c920ea6252b0b035d31b18e0115e0743d5ca97`  
		Last Modified: Tue, 17 Aug 2021 01:21:04 GMT  
		Size: 49.1 MB (49079655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcf1e19e8c366bbeed533597a718657c71c55ace29aedda5015330b7811605a`  
		Last Modified: Tue, 17 Aug 2021 20:57:20 GMT  
		Size: 7.3 MB (7252790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab553f775efe1ebe386c27726c3f1723f48e32fb8865b49e910c181e3cfab788`  
		Last Modified: Tue, 17 Aug 2021 20:57:21 GMT  
		Size: 10.0 MB (10016441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28044c83fd33e51894666e65c54e1691250d8298a8687b14d7a079df5afd69c`  
		Last Modified: Tue, 17 Aug 2021 20:58:09 GMT  
		Size: 50.8 MB (50843141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a254e959b3e0b79e2ecebd56f2318cd2299b7983a3afc46b2ccf4c7400d3cb`  
		Last Modified: Tue, 17 Aug 2021 21:00:16 GMT  
		Size: 179.9 MB (179911997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7d77d8233aa6421f8d2c87bb6223b501ea972fcff66e42cb2170bae155221c`  
		Last Modified: Wed, 18 Aug 2021 12:44:14 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efb27dd0bb359e886a5a050fdb6574c1275e0f1415722af0a2b0f98572c9150`  
		Last Modified: Wed, 18 Aug 2021 12:44:26 GMT  
		Size: 28.7 MB (28664051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69d72d9f7d3a92cdf511d5731a779c5c39c3a5bab49260f201f33ce76a71269`  
		Last Modified: Wed, 18 Aug 2021 12:44:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:045e158c519ed0e8b4faa0d20d36a9fe95ac392bd00837fc8f338742df975dd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.8 MB (362799020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3d6ecfe9727b8a30cad26e1704b84b6ccc4e0d59d50f995a940d32f7d8a2e5`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:33:35 GMT
ADD file:cd847762c4d814b1302366ad14c10c4fc83be52d52ede8336744b1f0bf988112 in / 
# Tue, 17 Aug 2021 01:33:40 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:57:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 15:00:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:22:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 06:13:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Aug 2021 06:13:33 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 06:13:36 GMT
ENV RUBY_MAJOR=3.0
# Wed, 18 Aug 2021 06:13:38 GMT
ENV RUBY_VERSION=3.0.2
# Wed, 18 Aug 2021 06:13:41 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Wed, 18 Aug 2021 06:18:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Aug 2021 06:18:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Aug 2021 06:18:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Aug 2021 06:18:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 06:19:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Aug 2021 06:19:25 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a4b39f6d7e8772c5450fb8b799577a194b8bdd1a2935d732d4836f0713e6518a`  
		Last Modified: Tue, 17 Aug 2021 01:47:16 GMT  
		Size: 54.2 MB (54182973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2ff2b66aeb977708310cb04f7b6110efbc73ff8a538b6f003df129f2fb0f3`  
		Last Modified: Tue, 17 Aug 2021 16:04:35 GMT  
		Size: 8.3 MB (8272123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edeeefbd9326b5c8dbf6c5b3a60d602c1e0f2d0af22dc2cfc28842351dc6b95`  
		Last Modified: Tue, 17 Aug 2021 16:04:33 GMT  
		Size: 10.7 MB (10727834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350768736925f68aafac882b13a3e7593640560819c88b60d0f566ec1781de0b`  
		Last Modified: Tue, 17 Aug 2021 16:05:58 GMT  
		Size: 57.5 MB (57457638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59be0c0011a56689a0699ad31ad26e9a7da01ae88b4764884cf262f2cb31c28`  
		Last Modified: Tue, 17 Aug 2021 16:10:04 GMT  
		Size: 203.3 MB (203284992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5151f1b0778b790402bd13f26fd225c762c5339f85fed58cbee7fb388268832`  
		Last Modified: Wed, 18 Aug 2021 06:44:10 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f091c97809793ba81a79026eef57d3fd6a14cd789af3c271a574cd2b1659680f`  
		Last Modified: Wed, 18 Aug 2021 06:44:14 GMT  
		Size: 28.9 MB (28873083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247bb2518b931f52ad122ef63fd1b4c686e22ce63d1cfe6708b042e90d12eae7`  
		Last Modified: Wed, 18 Aug 2021 06:44:10 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; s390x

```console
$ docker pull ruby@sha256:9cf2ec2dc1392144fcf5fd263dbdc40e3ba4e47644c3f8816be4678e3c8df57c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.2 MB (323188867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d553bfb8106e22d835c65ff0eb1be6cab681dc1004da3c27f5d56b993c61d836`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:25 GMT
ADD file:0443e797578f02bf4a9404844d217d992a5dafb634ae3a03ed9e181313f78d4c in / 
# Tue, 17 Aug 2021 01:49:33 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:34:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:34:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Aug 2021 07:35:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:37:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:59:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 12:59:05 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 12:59:05 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 12:59:06 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 12:59:06 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 13:01:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 13:01:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 13:01:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 13:01:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 13:01:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 13:01:30 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b14cfca9681354c01ba0c52718b98b1783ccc6a88170ff1b5d491a86f389ccee`  
		Last Modified: Tue, 17 Aug 2021 01:57:51 GMT  
		Size: 49.0 MB (49004330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398cc2dd69156863e1a916460d85ea681c1fea50e25611f3fa0bf634ecda0a97`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 7.4 MB (7400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bc3c2fc42de3b04bcd5e6a2d4b4004ba2295b0580a1ae1d2e01ea1d65200a0`  
		Last Modified: Tue, 17 Aug 2021 07:44:16 GMT  
		Size: 9.9 MB (9883198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723dbf1359b8c022bdec44c42d0fda155c8ca45da7152e885954f7c17d70c05c`  
		Last Modified: Tue, 17 Aug 2021 07:44:31 GMT  
		Size: 51.4 MB (51380299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0234edac00c22e8e9fac61c99ce359d2968b0d2eed6a0bc430c1312fcb980c`  
		Last Modified: Tue, 17 Aug 2021 07:45:00 GMT  
		Size: 176.9 MB (176877890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f072c04272c5f33c375b18b02b6731de09c173c18ea3c307c1bf097aca0b459`  
		Last Modified: Tue, 17 Aug 2021 13:27:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d24fac06860cb31c8fe471ad770b4063b2a50c822c3234dae8c40f2092a4952`  
		Last Modified: Tue, 17 Aug 2021 13:27:14 GMT  
		Size: 28.6 MB (28641986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e6c173245a765524fa78806d03f20ee335b2825a3456128eedfcb6540d4dfd`  
		Last Modified: Tue, 17 Aug 2021 13:27:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
