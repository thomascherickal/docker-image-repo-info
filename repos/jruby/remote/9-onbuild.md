## `jruby:9-onbuild`

```console
$ docker pull jruby@sha256:19abab2689a47e1b09acd1eafb55ae5798446e10d492c317ac8c35d50f6f2811
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jruby:9-onbuild` - linux; amd64

```console
$ docker pull jruby@sha256:1faf52b0d187b0ef363aa5e2d01bc3db0993877e8d4babf7f690dc8464d14160
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (266008779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2e6962ebb46c51abe802654e7369cd6ae5f50fbba63730e7527beee3e8752f`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:54:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:47:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:48:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sat, 10 Apr 2021 12:48:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Sat, 10 Apr 2021 12:48:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 12:48:58 GMT
ENV LANG=C.UTF-8
# Wed, 21 Apr 2021 21:55:58 GMT
ENV JAVA_VERSION=8u292
# Wed, 21 Apr 2021 21:56:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 21 Apr 2021 22:45:40 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 21 Apr 2021 22:45:40 GMT
ENV JRUBY_VERSION=9.2.17.0
# Wed, 21 Apr 2021 22:45:41 GMT
ENV JRUBY_SHA256=7701d3537b3a606d2765ac6d5c40e675ddaa01d3cebad26a21a66e3aadd5c202
# Wed, 21 Apr 2021 22:45:43 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 21 Apr 2021 22:45:43 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Apr 2021 22:45:44 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 21 Apr 2021 22:45:53 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 21 Apr 2021 22:45:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 21 Apr 2021 22:45:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 21 Apr 2021 22:45:54 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Apr 2021 22:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 21 Apr 2021 22:45:55 GMT
CMD ["irb"]
# Wed, 21 Apr 2021 22:46:53 GMT
RUN mkdir -p /usr/src/app
# Wed, 21 Apr 2021 22:46:53 GMT
WORKDIR /usr/src/app
# Wed, 21 Apr 2021 22:46:53 GMT
ONBUILD ADD Gemfile /usr/src/app/
# Wed, 21 Apr 2021 22:46:53 GMT
ONBUILD ADD Gemfile.lock /usr/src/app/
# Wed, 21 Apr 2021 22:46:53 GMT
ONBUILD RUN bundle install --system
# Wed, 21 Apr 2021 22:46:54 GMT
ONBUILD ADD . /usr/src/app
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44718e6d535d365250316b02459f98a1b0fa490158cc53057d18858507504d60`  
		Last Modified: Sat, 10 Apr 2021 02:01:57 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe9738af0cb2184ee8f3fb3dcb130455385aa428a27d14e1e07a5587ff16e64`  
		Last Modified: Sat, 10 Apr 2021 02:01:59 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37aabde37b87d272286df45e6a3145b0884b72e07e657bf1a2a1e74a92c6172`  
		Last Modified: Sat, 10 Apr 2021 02:02:22 GMT  
		Size: 51.8 MB (51841093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87fc504233c0bf4b90cb62e9b114fb0f1927b4a65265ffc153378d21aa8fe70`  
		Last Modified: Sat, 10 Apr 2021 12:58:46 GMT  
		Size: 5.3 MB (5286527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc62143cb8cc43e9daa5275171f9ec1d73ded74b3948173b66390184f4ee0656`  
		Last Modified: Sat, 10 Apr 2021 13:01:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646a47c88e4331d1da42c78785cbfd1cf6292a4ebaa7f5376695c39efbb4b757`  
		Last Modified: Wed, 21 Apr 2021 22:06:13 GMT  
		Size: 105.9 MB (105943615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5334794a2d857e4b18f5c7b081bf32c4e9da28c95b52764769d626dfd7fe9b0`  
		Last Modified: Wed, 21 Apr 2021 22:48:52 GMT  
		Size: 7.8 MB (7789610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0d5e9ade2af5418e470a6932e92e394dfed81a6a0682374f63c9f7a1d9a211`  
		Last Modified: Wed, 21 Apr 2021 22:48:54 GMT  
		Size: 25.9 MB (25856650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a77526d3c70784767bff2051adf309b6da121591fb7332fe6f9ffd03848a13`  
		Last Modified: Wed, 21 Apr 2021 22:48:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15237f709b349153c5bcceecc4b31c988e6325541832e9afcb226ddc8dc469b1`  
		Last Modified: Wed, 21 Apr 2021 22:48:52 GMT  
		Size: 1.0 MB (1027408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebeb7a2ec1ed8b67faff0ed5cd52e921dbcf64d6f6aa918f7c95bac188af94bb`  
		Last Modified: Wed, 21 Apr 2021 22:48:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb46f54683ec7acf9aaadc05ded6b1904a26b50c15b83a32062176a53efbe56`  
		Last Modified: Wed, 21 Apr 2021 22:49:59 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
