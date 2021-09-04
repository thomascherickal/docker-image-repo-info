## `ruby:3-slim-buster`

```console
$ docker pull ruby@sha256:38c76f619e387db96713f94e1b31df19544e9b502ae9c601b17b5c6a2595d62b
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

### `ruby:3-slim-buster` - linux; amd64

```console
$ docker pull ruby@sha256:7f89a293287b9b8a940bf8bc5c78af4735fd752743b575626c07ac13b7a020fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68138289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6cdd8a09046d49a2d34ce1525c846340477abd9e7e64441a5fb21239745642`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 14:17:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 14:17:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 14:17:25 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:17:25 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 14:17:25 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 14:17:26 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 14:22:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:22:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:22:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:22:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:22:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:22:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838595e1819d0a229d6d8498720ca7bb441ff298e42d4aa628ad8fa44f45666d`  
		Last Modified: Fri, 03 Sep 2021 14:57:39 GMT  
		Size: 12.6 MB (12564965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533c3020e404ee01e2192449746f4de04f9ba5e9ee73cb621e90deea15d31430`  
		Last Modified: Fri, 03 Sep 2021 14:57:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5701a9b75326a07b397fe6dcb74de396b4585d9e84e9fbdd6088e50778369`  
		Last Modified: Fri, 03 Sep 2021 14:57:39 GMT  
		Size: 28.4 MB (28427111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855ed945b13e5b80d95dac4348bb64ab6f9e7f975ceab2781153b082cffcaff2`  
		Last Modified: Fri, 03 Sep 2021 14:57:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:abcf81d8d3c9b6c7245e38e69ebe418a034a5500da1ede869c735b852eac3527
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62734310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4f27cad82c4de19b11aea05410e2a6d138b3f344eb3dfa5c0fbc16119ba453`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:13:23 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 17:13:24 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 17:13:24 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 17:18:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:18:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:18:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:18:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:18:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:18:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34869eb745a2f1bb1491ef7915fde3af386e0d88494010619959392cc9ffd27`  
		Last Modified: Fri, 03 Sep 2021 17:59:56 GMT  
		Size: 27.5 MB (27505986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85f5e691daaff43b8333d8fec0d343d1cc6e293a705afa755f81d19fd69a483`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:f0560e4b026bc94261fff843cd5b37872301c8845c032d1ce492051c92ab4aeb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60011527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430dcef1d88ec4274609dc3bbe6cb318bec7187337332663093f535b1fa011db`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 01:00:40 GMT
ADD file:4754bbccf4c59f77dd54f3888871f0635a2f9655cda53f50e63237f1580286e0 in / 
# Fri, 03 Sep 2021 01:00:41 GMT
CMD ["bash"]
# Sat, 04 Sep 2021 05:06:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:06:42 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Sep 2021 05:06:42 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 05:06:43 GMT
ENV RUBY_MAJOR=3.0
# Sat, 04 Sep 2021 05:06:43 GMT
ENV RUBY_VERSION=3.0.2
# Sat, 04 Sep 2021 05:06:44 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Sat, 04 Sep 2021 05:11:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Sep 2021 05:11:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Sep 2021 05:11:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Sep 2021 05:11:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Sep 2021 05:11:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Sep 2021 05:11:25 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2215ad7863d95c38f1f794f1d5b4d6c5ca4ca7e921e4bb7218b803f7ed270675`  
		Last Modified: Fri, 03 Sep 2021 01:16:23 GMT  
		Size: 22.7 MB (22746151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd659f21a6c01cd37d44848dfa252be1e606e96dc6eae454c9a3b30230a931ee`  
		Last Modified: Sat, 04 Sep 2021 06:06:06 GMT  
		Size: 9.9 MB (9873027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfbc24d05836091720d75dadba41b753c1338d0e7243fc616ddf775ae0d1c25`  
		Last Modified: Sat, 04 Sep 2021 06:05:59 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30bba35632c48bcca938fc8767a2ab253c78ffeeb0b289fbea67f8891221583`  
		Last Modified: Sat, 04 Sep 2021 06:06:10 GMT  
		Size: 27.4 MB (27391978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1bff473f153564aa34dea60d509de4efbb1fd500e8b0c30e41176058d43d66`  
		Last Modified: Sat, 04 Sep 2021 06:05:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:146f9e5b55706119493cf0f5b066191049d6a6d5d34e4209001bf7e7b973984b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65337032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b05dfc2a1101f65a88b7d5ab704d211b248ed691950f84bda84b123596c92a86`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:01:36 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 12:01:37 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 12:01:37 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 12:04:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:04:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:04:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:04:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:04:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:04:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f789fdfb8725726715e5ab7b7f72adedb101850d27fc9fb267b9790fe3a07cc7`  
		Last Modified: Fri, 03 Sep 2021 12:26:55 GMT  
		Size: 28.2 MB (28157397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2dc36df757afc59e6a448589e5aeb729432c9425890d3133bcbff88b5ebd9b`  
		Last Modified: Fri, 03 Sep 2021 12:26:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; 386

```console
$ docker pull ruby@sha256:1e1dc2b9c0d64a3a7b356a9f4dc18d34ed83cfb2509ced8458aed01437a8dd88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0cb271b9b5614b20aae724d99366a0a885c7e7b8d3d5e113f0815a4a6fe41e2`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:21:09 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 11:21:10 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 11:21:10 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 11:26:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:26:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:26:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:26:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:26:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:26:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0370d22021ccf99dc48999da91a477545cb3f51cf3d2eb309bf11031898c527c`  
		Last Modified: Fri, 03 Sep 2021 12:08:34 GMT  
		Size: 27.7 MB (27711722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bc0c36d037db50d70df2bd46a1388d8727cdbd194cb13ff774a036cf991176`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; mips64le

```console
$ docker pull ruby@sha256:7a846fa7abafb09e10378b465708368e3027dbd654823bb9b10cd11401be08dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66067184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6eec93fdcbfa2afb4b51d69a5d6cbf177ac27899bf2d40a91cc50b8fba9bce8`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 17 Aug 2021 01:12:26 GMT
ADD file:8bd279803ead4ddce8db90b65e89c423f84fbf6042bfbeae8c09486b2e884cde in / 
# Tue, 17 Aug 2021 01:12:27 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 13:05:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:05:41 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 13:05:42 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 13:05:42 GMT
ENV RUBY_MAJOR=3.0
# Tue, 17 Aug 2021 13:05:42 GMT
ENV RUBY_VERSION=3.0.2
# Tue, 17 Aug 2021 13:05:42 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Tue, 17 Aug 2021 13:15:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 13:15:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 13:15:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 13:15:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 13:15:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 13:15:37 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:a711e3e37b88ef77496c07ed663bb4270ecba9057eba452a91cc9be0bafb9c32`  
		Last Modified: Tue, 17 Aug 2021 01:21:44 GMT  
		Size: 25.8 MB (25813007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cf03c95787660b404a097ee35b25ddb3bc7b823c1f5d8f216119b64d5fe235`  
		Last Modified: Tue, 17 Aug 2021 14:07:43 GMT  
		Size: 11.6 MB (11627872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3d773e4abd3ddec22a7b6cf7364af59b77f4a38329958192373e952c51c732`  
		Last Modified: Tue, 17 Aug 2021 14:07:32 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d9fe060c3b332ea8f5a6e211f86986ddd127ae16c703ec670a478485b8210c`  
		Last Modified: Tue, 17 Aug 2021 14:07:45 GMT  
		Size: 28.6 MB (28625964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa34f9249c834bd5163b1312a06b0751860c266b3ac4e481d2e27bb9db08a8c`  
		Last Modified: Tue, 17 Aug 2021 14:07:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:67aad30809703a50cb3c26e960b49b24ddbe350b550a45a86b21631961190a16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.1 MB (72115462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f588090e65689badde7d42eb7bf43becb701d3cf9318743a0033dec766222f4`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:33 GMT
ADD file:6c1662ddb92232ae8969a86a18dacab97b3b5792a1ecda49e6ac741a1a5c878c in / 
# Fri, 03 Sep 2021 01:24:41 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 19:43:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 19:43:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 19:43:55 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 19:44:03 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 19:44:08 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 19:44:11 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 19:56:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 19:56:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 19:56:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 19:56:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 19:57:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 19:57:18 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8258146296247df1f308a336d4abf286afae14e3375edefb87a091e80745e29f`  
		Last Modified: Fri, 03 Sep 2021 01:39:45 GMT  
		Size: 30.6 MB (30553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79608f343b1abc29aa36a5a888c5669cd7714921be23b234ae70ef00fe5ce91`  
		Last Modified: Fri, 03 Sep 2021 21:07:40 GMT  
		Size: 12.7 MB (12705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f1b01f4719066c36c3591ad469d2d73fac09969547ef89f16d42f5bfaf8b6f`  
		Last Modified: Fri, 03 Sep 2021 21:07:37 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ac840f95aefe7afd2f8cfa324ec2a6b4184288154ba6d296b7323d60ea867e`  
		Last Modified: Fri, 03 Sep 2021 21:07:41 GMT  
		Size: 28.9 MB (28855871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52454b9d23a81c8d2d12ab29a178f31a7b6aa71f6fa3f776820d1c2300a7e578`  
		Last Modified: Fri, 03 Sep 2021 21:07:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-slim-buster` - linux; s390x

```console
$ docker pull ruby@sha256:eae71e2bde695c90beb80ff78c2a827dd88379285442210d6a2d108b32e65b74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65199913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dbefa67cbdbb499c3cb057a03f8a3447ec02ba5a211ab9fba6eee6b7e87ceb0`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:10:18 GMT
ENV RUBY_MAJOR=3.0
# Fri, 03 Sep 2021 13:10:18 GMT
ENV RUBY_VERSION=3.0.2
# Fri, 03 Sep 2021 13:10:19 GMT
ENV RUBY_DOWNLOAD_SHA256=570e7773100f625599575f363831166d91d49a1ab97d3ab6495af44774155c40
# Fri, 03 Sep 2021 13:14:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:14:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:14:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:14:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:14:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:14:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8674ed28fcf11410f62873091e5e320b90a63dfbea3a0cf225deed27d3cba3f`  
		Last Modified: Fri, 03 Sep 2021 14:13:13 GMT  
		Size: 28.6 MB (28623500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b649080718aa4a8a417f6aaf7860dc3c47002bb848f76777c86545a83cb4219`  
		Last Modified: Fri, 03 Sep 2021 14:13:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
