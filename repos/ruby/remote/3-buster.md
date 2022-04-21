## `ruby:3-buster`

```console
$ docker pull ruby@sha256:64f4fb6c69e3cbab0cf48ae6980ecc04071688c4533569d3376bee4f28ac1a44
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
$ docker pull ruby@sha256:081adae95bb48183cd78a02798341904e6637eef257ab66e205cf9fcd65f2a20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344911352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cd67133783ab4357b4c681b4465dfb751d524f531fb215e022320559e0391d`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:59:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:59:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:59:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:00:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:51:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 13:51:14 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 14:00:34 GMT
ENV RUBY_MAJOR=3.1
# Wed, 20 Apr 2022 14:00:34 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 20 Apr 2022 14:00:34 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 20 Apr 2022 14:02:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 14:02:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 14:02:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 14:02:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 14:02:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 14:02:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdd409f4b2bf3771fac1cbc2df46d1cbb4b800b154cfc33e8e0cd23e67ab3e0`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 7.9 MB (7856378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3069e6cecf9d5e43ace0a925b53849b2fd189ef41883d45d8f2e12213c2c06`  
		Last Modified: Wed, 20 Apr 2022 07:06:56 GMT  
		Size: 10.0 MB (9997231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee16f45eff97cbe98b74c63ca2375b2c6b2592cd765a86df098f731baab13ad`  
		Last Modified: Wed, 20 Apr 2022 07:07:14 GMT  
		Size: 51.8 MB (51843794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cee68386155951f51cf2088092ed4b624b2ba9c36b2ec378ab041cb5bcea514`  
		Last Modified: Wed, 20 Apr 2022 07:07:48 GMT  
		Size: 192.6 MB (192640130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c58f08462b8a443c8016636439e03fbb4d6d4f6a7d15754f4d9d14bf8ffa5`  
		Last Modified: Wed, 20 Apr 2022 14:31:15 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6720a7b47dfea495b97a830ffca855a7c1e3626b9653fce434a8787d0272c134`  
		Last Modified: Wed, 20 Apr 2022 14:32:43 GMT  
		Size: 32.1 MB (32136458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6058bd828d8f5e96ac220a5bc810fd9142996e8cd54874d50b9da88c6886c66`  
		Last Modified: Wed, 20 Apr 2022 14:32:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:ffa2f788ff8683073e7224db96d41b550c16fb6a6dc3de51a8151d9062d21b2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.2 MB (317180746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26dda4ae18b030706733995cabd05913cebd55a1df3923e3001352fa60fb701b`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:11 GMT
ADD file:ad329516525d9a2e9eecb4bd6263809faafa65bbd9e6deebcda8196b0ea24234 in / 
# Wed, 20 Apr 2022 07:17:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:42:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:43:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 12:44:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:46:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:17:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 21:17:05 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 21:38:15 GMT
ENV RUBY_MAJOR=3.1
# Wed, 20 Apr 2022 21:38:15 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 20 Apr 2022 21:38:15 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 20 Apr 2022 21:42:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 21:42:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 21:42:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 21:42:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 21:42:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 21:42:48 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d426a13b8d217ec7cc2eceea9d798d79a1c36c60cb9363d2ef2d86abcf895e88`  
		Last Modified: Wed, 20 Apr 2022 07:33:13 GMT  
		Size: 48.2 MB (48153607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e6f91f8d8f6effa3b0301678a3bffa5959462bbf96deb2b669b6388e93d47d`  
		Last Modified: Wed, 20 Apr 2022 13:04:28 GMT  
		Size: 7.4 MB (7400330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f92b3ddeebddc859cc64404c00806ebf416f52030af1bc22996ce6b6099f8e`  
		Last Modified: Wed, 20 Apr 2022 13:04:28 GMT  
		Size: 9.7 MB (9687491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33f3b87e965d4f4f6a012d5312fa273c2beffba18ccb2041fb9fe8fa446ee13`  
		Last Modified: Wed, 20 Apr 2022 13:05:16 GMT  
		Size: 49.6 MB (49577569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c69a511bd7de27d16243999eaf3cb72eed709eb72e10c0bdd344b7ec060a1d`  
		Last Modified: Wed, 20 Apr 2022 13:07:13 GMT  
		Size: 171.6 MB (171575879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cf528f3eeedd7382d600a5131f620fd109cdb7b5e72f048d780e26805475d1`  
		Last Modified: Wed, 20 Apr 2022 22:50:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f17bb418e4aa8ed8bfa69ab3b0421d3aa2f6c2512c730835d1f8c14ada4656`  
		Last Modified: Wed, 20 Apr 2022 22:52:49 GMT  
		Size: 30.8 MB (30785496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a357fc9de19556c821848331332da1e821f79c1649bc1eca83737504b4aa30`  
		Last Modified: Wed, 20 Apr 2022 22:52:41 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:eea0abb6c5ad9e72069a10fb68a2d3ab1a058258e3c4022655fa00f4b61f92a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309124646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ecdbabb7583dc7ef237fed825a11ea33f5324a9f6fea4df70f1925067f1781`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 02:19:04 GMT
ADD file:60a690e302d164c569e6f3fc29adb6686618bb728249405f90960835525b0599 in / 
# Tue, 29 Mar 2022 02:19:06 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:09:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:10:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:10:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:13:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 15:50:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 31 Mar 2022 15:50:01 GMT
ENV LANG=C.UTF-8
# Thu, 31 Mar 2022 15:50:01 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 19:09:58 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 19:09:59 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 19:14:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:14:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:14:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:14:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:14:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:14:22 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:0cc72482f2e040b686190f2967010d45947924353440070552a298b9f9f81b19`  
		Last Modified: Tue, 29 Mar 2022 02:34:54 GMT  
		Size: 45.9 MB (45914531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ee42f432eca8b10b5cc28da57027f157052392220ed81ab477a06ce1771abe`  
		Last Modified: Wed, 30 Mar 2022 21:33:01 GMT  
		Size: 7.1 MB (7144979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bdeb2a3bd0d310e035553bfd8dca244c71e5c1d7fa33c8e1f19d5912e0be7e`  
		Last Modified: Wed, 30 Mar 2022 21:33:02 GMT  
		Size: 9.3 MB (9343870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd207bbebe5d300d8201e2319d4779866fb17a8c6da7f336642683ead787209`  
		Last Modified: Wed, 30 Mar 2022 21:33:46 GMT  
		Size: 47.4 MB (47359089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22e994f86d86dc3f616423bad52a5522a31743b53cdbdbc8dcd39c226b1f5d`  
		Last Modified: Wed, 30 Mar 2022 21:35:33 GMT  
		Size: 168.7 MB (168687691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf86cdddd4bdac4cc673549ecce7d48d9d3008f586c766e8330e6520fcfaff6`  
		Last Modified: Thu, 31 Mar 2022 16:28:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956b55f7707d5c7e59cbadf8bc1e908091e870c1c9fb814332757b425df4c235`  
		Last Modified: Tue, 12 Apr 2022 20:57:30 GMT  
		Size: 30.7 MB (30674111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8018f2043023232d98c8f506acfc5c08bd480cd54efc535495cff03800f1e814`  
		Last Modified: Tue, 12 Apr 2022 20:57:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:2dcdb64504689dfd968de5c41f1efde92d41f6b04fcbee04c16f52ac8f7da431
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.4 MB (334402254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f02e1020d12b9135a6873364cdf501a968594f62acab8184f8f84d2a02959e77`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:45:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:45:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:46:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:26:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 12:26:49 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:36:15 GMT
ENV RUBY_MAJOR=3.1
# Wed, 20 Apr 2022 12:36:16 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 20 Apr 2022 12:36:17 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 20 Apr 2022 12:38:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 12:38:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 12:38:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 12:38:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 12:38:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 12:38:17 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80651adb7e52d8ecd27d43b9e69ada9ca277071ea09607121d0076de36480b`  
		Last Modified: Wed, 20 Apr 2022 06:55:25 GMT  
		Size: 7.7 MB (7719745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b38ee622cbfb492ebc3bc598771624fba7ef1830b4e0f9737f2bbf4b6ec0ea`  
		Last Modified: Wed, 20 Apr 2022 06:55:26 GMT  
		Size: 9.8 MB (9767312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc937997baec7d2d040aba23614db074862008cbdd69b46d2baea31711d58a50`  
		Last Modified: Wed, 20 Apr 2022 06:55:45 GMT  
		Size: 52.2 MB (52174549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d799cbd560490faf9e2001aa60899c29713ab4bc6af30427e08f9b79b39244b4`  
		Last Modified: Wed, 20 Apr 2022 06:56:19 GMT  
		Size: 184.1 MB (184142825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a6c3f392859d0ac6a9c0bca66b682f8b0a7759c32f874afdbdc4a7aef5281`  
		Last Modified: Wed, 20 Apr 2022 13:09:15 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfdacb98cbe3034775623cda5ad05872f71f8b026f178ed5eacf8997014b25c`  
		Last Modified: Wed, 20 Apr 2022 13:10:55 GMT  
		Size: 31.4 MB (31369746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd0206a4abf1ae9f116daffa7593e4621f492580aee7cb875b1f971e24379ff`  
		Last Modified: Wed, 20 Apr 2022 13:10:52 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; 386

```console
$ docker pull ruby@sha256:b7cd4b024083eaa3cab5bcd1be367acc7c26ca9ec948934c98a20418ac72cdba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.6 MB (352639067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68cb306a22f10110d509cb19053268d87b91b367fcd84d9332d9a21fc620da1`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:47 GMT
ADD file:f66ba5e7b2801d19041661506f244a3bb89fc613e2e27891bdba3183bd6ee097 in / 
# Wed, 20 Apr 2022 07:37:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:17:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:18:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:18:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:20:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:26:56 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 16:26:57 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 16:36:39 GMT
ENV RUBY_MAJOR=3.1
# Wed, 20 Apr 2022 16:36:40 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 20 Apr 2022 16:36:41 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 20 Apr 2022 16:38:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 16:38:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 16:38:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 16:38:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 16:38:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 16:38:35 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:6e8f333ddc9f58dd9e74b1f250e3812ba3942ef13abee1d6b4e3d3131a7e29ff`  
		Last Modified: Wed, 20 Apr 2022 07:45:17 GMT  
		Size: 51.2 MB (51195868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4353b7b00b407b29561abe4d0fffed162775a58e3c48ee2edf64cbb21cfcb11`  
		Last Modified: Wed, 20 Apr 2022 10:28:45 GMT  
		Size: 8.0 MB (8022285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f90dfd06367deaf8c4c4f802c2dfb9a36dbfb3d208f4972a8c79b0892b07832`  
		Last Modified: Wed, 20 Apr 2022 10:28:45 GMT  
		Size: 10.1 MB (10122004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71948e43ad88935c94f9d58f3ef1c3f9aeca8f23d363ae038a1e4ad7d5ff8e52`  
		Last Modified: Wed, 20 Apr 2022 10:29:05 GMT  
		Size: 53.4 MB (53443227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b68088036730eb63d8a89738d8711d9c5f333e0667cf48d8a0194194c3bc9f`  
		Last Modified: Wed, 20 Apr 2022 10:29:39 GMT  
		Size: 199.1 MB (199121303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c492888876deb3bff4a95ffdbe9a9b83879c0827ae9c3804136175b75816b11e`  
		Last Modified: Wed, 20 Apr 2022 17:10:48 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4f07c8a892184a778db5250bb0b9b360c382eebc7365015eee4cd7ce487e8c`  
		Last Modified: Wed, 20 Apr 2022 17:12:44 GMT  
		Size: 30.7 MB (30734037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea33a1778891b8f441b83439218414181866719292db1db9a5ff709c9dd4ebc`  
		Last Modified: Wed, 20 Apr 2022 17:12:37 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:a8fccb39a46365a2a22b8658d4b5d58b6aba33470ab85536c45110ed9893c777
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328917653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be1dcd6cefe026452254eac7cc0ff5ec6c5dded7b3ca3db7de720b796cabd576`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:01 GMT
ADD file:c86010b52f782f910842586e6abc81e64c7a659d001b89799314a59f4fb96573 in / 
# Tue, 29 Mar 2022 07:43:06 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:36:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:38:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:44:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:09:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 30 Mar 2022 23:09:18 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 23:09:24 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 19:33:42 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 19:33:48 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 19:44:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:44:17 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:44:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:44:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:44:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:44:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8e0bee9c4b9257c0ad7469830be5e890536feef4e8ffe6c2613b7e8be7e060f6`  
		Last Modified: Tue, 29 Mar 2022 07:53:41 GMT  
		Size: 49.1 MB (49079891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc690a0cd1092524bdd12063c730cdf1df3dfa2f8c5920231d8477654c04b854`  
		Last Modified: Tue, 29 Mar 2022 09:38:05 GMT  
		Size: 7.3 MB (7272773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe0e6a034874e5b70e892d14e911e5aaa7f314b7588616996be6ff22190b1a`  
		Last Modified: Tue, 29 Mar 2022 09:38:06 GMT  
		Size: 9.8 MB (9800273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84f8d8d66208e065df79ad5efc3776584f6dd13891c8f9eafa9c02a12aaf58`  
		Last Modified: Tue, 29 Mar 2022 09:38:52 GMT  
		Size: 50.9 MB (50859745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13876620bf13ddb0a90ac352ea4aa991b4215b6d3e91eb84e189559155991d28`  
		Last Modified: Tue, 29 Mar 2022 09:40:54 GMT  
		Size: 180.0 MB (180013664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cf229f569ed11b48dc9d127d4bb4f48b17d247826b812e2d849da9b4c1598e`  
		Last Modified: Thu, 31 Mar 2022 01:40:35 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628ba0fd95e668c3fb5efbc4c5705b34394b39c0a439bd59c4532e2b563a3474`  
		Last Modified: Tue, 12 Apr 2022 22:04:57 GMT  
		Size: 31.9 MB (31890965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b075400c0b0491fad1d1694b315f9e71735655581bce80a07314aade25652864`  
		Last Modified: Tue, 12 Apr 2022 22:04:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:2e7cbf9872a9307374d983b0c3b4920058378c2c2ee5344353b2e3b95f55c6ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.3 MB (366344640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6897c592416c7762e79371caa9896e3ec2b51ec5cf5bd57090c2833d47cd9bd5`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:25 GMT
ADD file:a600709d679cffd058d04ba0eb0765cc870766fd5de083ada0eeccfd7afc21f8 in / 
# Tue, 29 Mar 2022 00:22:30 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:59:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:59:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 06:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 06:09:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 06:45:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 31 Mar 2022 06:45:29 GMT
ENV LANG=C.UTF-8
# Thu, 31 Mar 2022 06:45:38 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:55:02 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:55:12 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 19:01:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:01:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:01:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:01:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:02:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:02:20 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:eb53bdc4c2c6ececbd424b1c643b9877934a5297a5d2db0eca1a175d7a21d32e`  
		Last Modified: Tue, 29 Mar 2022 00:33:53 GMT  
		Size: 54.2 MB (54183100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596f9130bbf698f182cdd8f8965c6d1fb059aff38e309f7dd44db12967d4ab7a`  
		Last Modified: Wed, 30 Mar 2022 06:27:07 GMT  
		Size: 8.3 MB (8293334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf74211bc82c5c0431e1ac0b76c006093e829ef420568923567cb2d6bf07a69`  
		Last Modified: Wed, 30 Mar 2022 06:27:07 GMT  
		Size: 10.7 MB (10727786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0360cd705f30cbb5b19634dbb8790f95b284fad0f6221eddc372edc5c47b3d7b`  
		Last Modified: Wed, 30 Mar 2022 06:27:32 GMT  
		Size: 57.5 MB (57457953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254f54f18ff34ed3bbde96d1961198e167a41e00fe59b38840fa0794b0742437`  
		Last Modified: Wed, 30 Mar 2022 06:28:18 GMT  
		Size: 203.4 MB (203372781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c60fa63b7c3836426c41fdcbcfc7b8681a0d8131820a7dbb86da902ff268ec`  
		Last Modified: Thu, 31 Mar 2022 07:39:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8627150e07170e25d6f6b9f25f9c3a653f5cc88b9d999de10896fa2f837484`  
		Last Modified: Tue, 12 Apr 2022 21:16:24 GMT  
		Size: 32.3 MB (32309310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71327b5bba5525c72b0e0bdd16786690246c02345c68c720b24d8f97e03ed896`  
		Last Modified: Tue, 12 Apr 2022 21:16:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-buster` - linux; s390x

```console
$ docker pull ruby@sha256:e6055bef972d02901e0a3460b595f3cfe7182276ec761ee75b0ebcc754572894
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326898226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a56768a9d96cca9b214ad471ef8c6ef29687421fbd82ee61fcba9d7172904e0`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:05 GMT
ADD file:fedc64967d4810188e8bd8289de1b1848a9501e7c68ae5bd4af83377fb9e3108 in / 
# Wed, 20 Apr 2022 08:40:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:17:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:18:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:20:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 18:16:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 18:16:10 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 18:30:10 GMT
ENV RUBY_MAJOR=3.1
# Wed, 20 Apr 2022 18:30:10 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 20 Apr 2022 18:30:11 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 20 Apr 2022 18:33:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 18:33:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 18:33:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 18:33:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 18:33:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 18:33:25 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5c2799a5996f1eb24bb7f4c0219facf7e95c780314bb9e9b62594f1fe56cd511`  
		Last Modified: Wed, 20 Apr 2022 08:49:56 GMT  
		Size: 49.0 MB (48999225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346950f736889109f89f84157f4d1cc4e75599b0df1eaf097803680eb2fdb900`  
		Last Modified: Wed, 20 Apr 2022 11:29:06 GMT  
		Size: 7.4 MB (7423732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a4abb2c4bda3be6e461f0d80740f3e2644a6dd833bcc0b97c83bd6a4e68ff`  
		Last Modified: Wed, 20 Apr 2022 11:29:06 GMT  
		Size: 9.9 MB (9883312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e0b9ea3498ff104383beba3cd632c64041234400c7a7d71acbcc7aa941e3a9`  
		Last Modified: Wed, 20 Apr 2022 11:29:21 GMT  
		Size: 51.4 MB (51383923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bfb5a5a189051fbcdf9ab35863372f16b29e414f52c171cdb6625e439f8fe8`  
		Last Modified: Wed, 20 Apr 2022 11:29:48 GMT  
		Size: 177.1 MB (177138032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b861adaf0d923b8859cace8cc365653e5715307f10c3fb4cc47154bca44b21`  
		Last Modified: Wed, 20 Apr 2022 19:21:19 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46af1971a5315db97741e741f3367acec1ed4b3d83121abf1e32b7c72742d33`  
		Last Modified: Wed, 20 Apr 2022 19:22:42 GMT  
		Size: 32.1 MB (32069627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45ef5ecd6999a6cb6ee5377323feb6c7b9a03989352c476c8aef37ac7cf4f3`  
		Last Modified: Wed, 20 Apr 2022 19:22:39 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
