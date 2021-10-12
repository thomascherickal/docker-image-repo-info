<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `jruby`

-	[`jruby:9`](#jruby9)
-	[`jruby:9.2`](#jruby92)
-	[`jruby:9.2.19`](#jruby9219)
-	[`jruby:9.2.19.0`](#jruby92190)
-	[`jruby:9.2.19.0-jdk`](#jruby92190-jdk)
-	[`jruby:9.2.19.0-jdk11`](#jruby92190-jdk11)
-	[`jruby:9.2.19.0-jdk17`](#jruby92190-jdk17)
-	[`jruby:9.2.19.0-jdk8`](#jruby92190-jdk8)
-	[`jruby:9.2.19.0-jre`](#jruby92190-jre)
-	[`jruby:9.2.19.0-jre11`](#jruby92190-jre11)
-	[`jruby:9.2.19.0-jre8`](#jruby92190-jre8)
-	[`jruby:9.2.19.0-onbuild`](#jruby92190-onbuild)
-	[`jruby:9.2.19-jdk`](#jruby9219-jdk)
-	[`jruby:9.2.19-jdk11`](#jruby9219-jdk11)
-	[`jruby:9.2.19-jdk17`](#jruby9219-jdk17)
-	[`jruby:9.2.19-jdk8`](#jruby9219-jdk8)
-	[`jruby:9.2.19-jre`](#jruby9219-jre)
-	[`jruby:9.2.19-jre11`](#jruby9219-jre11)
-	[`jruby:9.2.19-jre8`](#jruby9219-jre8)
-	[`jruby:9.2.19-onbuild`](#jruby9219-onbuild)
-	[`jruby:9.2-jdk`](#jruby92-jdk)
-	[`jruby:9.2-jdk11`](#jruby92-jdk11)
-	[`jruby:9.2-jdk17`](#jruby92-jdk17)
-	[`jruby:9.2-jdk8`](#jruby92-jdk8)
-	[`jruby:9.2-jre`](#jruby92-jre)
-	[`jruby:9.2-jre11`](#jruby92-jre11)
-	[`jruby:9.2-jre8`](#jruby92-jre8)
-	[`jruby:9.2-onbuild`](#jruby92-onbuild)
-	[`jruby:9.3`](#jruby93)
-	[`jruby:9.3.0`](#jruby930)
-	[`jruby:9.3.0.0`](#jruby9300)
-	[`jruby:9.3.0.0-jdk`](#jruby9300-jdk)
-	[`jruby:9.3.0.0-jdk11`](#jruby9300-jdk11)
-	[`jruby:9.3.0.0-jdk17`](#jruby9300-jdk17)
-	[`jruby:9.3.0.0-jdk8`](#jruby9300-jdk8)
-	[`jruby:9.3.0.0-jre`](#jruby9300-jre)
-	[`jruby:9.3.0.0-jre11`](#jruby9300-jre11)
-	[`jruby:9.3.0.0-jre8`](#jruby9300-jre8)
-	[`jruby:9.3.0-jdk`](#jruby930-jdk)
-	[`jruby:9.3.0-jdk11`](#jruby930-jdk11)
-	[`jruby:9.3.0-jdk17`](#jruby930-jdk17)
-	[`jruby:9.3.0-jdk8`](#jruby930-jdk8)
-	[`jruby:9.3.0-jre`](#jruby930-jre)
-	[`jruby:9.3.0-jre11`](#jruby930-jre11)
-	[`jruby:9.3.0-jre8`](#jruby930-jre8)
-	[`jruby:9.3-jdk`](#jruby93-jdk)
-	[`jruby:9.3-jdk11`](#jruby93-jdk11)
-	[`jruby:9.3-jdk17`](#jruby93-jdk17)
-	[`jruby:9.3-jdk8`](#jruby93-jdk8)
-	[`jruby:9.3-jre`](#jruby93-jre)
-	[`jruby:9.3-jre11`](#jruby93-jre11)
-	[`jruby:9.3-jre8`](#jruby93-jre8)
-	[`jruby:9-jdk`](#jruby9-jdk)
-	[`jruby:9-jdk8`](#jruby9-jdk8)
-	[`jruby:latest`](#jrubylatest)

## `jruby:9`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jdk`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jdk11`

```console
$ docker pull jruby@sha256:e46f46241a032fdf39a0acffe37e8b6ebff3abc90a9d4b0a0419d5907103673e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:57520b31d3fa224b3f32e19a57e5daf625d36652b92eb7d4fdf33c902a4f848f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.7 MB (363715350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a1cd4436e26b69d2744ea3050990c26598f80cfa81da4a32fae19f5b7d2e6a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:15 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe27974885e6146202139d340f9d214007f05c4fe92ee165893df2fd1349fb`  
		Last Modified: Wed, 29 Sep 2021 08:51:06 GMT  
		Size: 26.4 MB (26356058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f058f16ef05cefa0c10ad38f45972ea136eecd8aa2cfa3c983f2323b24812acf`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f883211ee83ac2b9e6f858dac22726dd0f859a12953f08912af64c7b6a8f4b6`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 1.0 MB (1026802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ba351a88f6273e468ea62357477753f57ba4534d3d022bad2aec4616c4e53`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jdk17`

```console
$ docker pull jruby@sha256:0b338c9487dbb3c483a37b9f88a37f7e151376fb2cd8be930a2eb84e04ff8bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b1374e40da9fe2cd7c6ce4732013681b8a0d0f9fb4588cdaa1d86bc2f58addd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.5 MB (356481056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f1b7a3235d708e688baba164cb95a342fda9b3f1e5e238ac6e6fd62741c94`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:32 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:33 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:42 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:44 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae164902b2e9d3ad535240b63971b8fc137124a8c3538816d4d5233c203e73`  
		Last Modified: Wed, 29 Sep 2021 08:51:22 GMT  
		Size: 26.4 MB (26356030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8520778aaca4506cb538b252ad3893632b13d6814bb57e7747292d8eee722`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe542002860439319b0d002610bd065c7be3dda1db8de9e66b30e4c6a1cce0d`  
		Last Modified: Wed, 29 Sep 2021 08:51:20 GMT  
		Size: 1.0 MB (1026782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc8225ae8eaaa696a6d62f0114b6d4b871a7ddd67940820f205a1317206415`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jdk8`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jre`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jre` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jre11`

```console
$ docker pull jruby@sha256:867ac9cb916f2549a9cc07964cc9e6f23eafca2bd53fbd7bb6e54771f8b5bfed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:94f519a48b6a8eb1118b13f73d05500f9251b62973414e7fa380ac2ad9dd03b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155826436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54fe08f7ef2ea5f938f8eb517261f6b3573de99415ddb5c5a6aaa45d0c2149d`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:56 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:56 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:57 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:07 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:08 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6ba890896c717ec3fc3486f7fc8038cce6c8855b7380ce815e3fcef9e3d9c`  
		Last Modified: Wed, 29 Sep 2021 08:50:51 GMT  
		Size: 26.4 MB (26355822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29610e4a43a92c762d00afdcf506d6772fb88fa09edc9941c4130287daa55a94`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5fa62cd9cfeb7738816def763478d6ebfeaca5b947a5e14759fbf807b23041`  
		Last Modified: Wed, 29 Sep 2021 08:50:49 GMT  
		Size: 1.0 MB (1026797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1760bdc9239d6efc6b23066c8c28f1e7ae9d2cb843ca8bcbf10bf3f278da496d`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-jre8`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19.0-onbuild`

```console
$ docker pull jruby@sha256:4c2a878dc1366a1125ad72dd694e7004fef2e538ef058cc1a0d6274d3c9ba765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19.0-onbuild` - linux; amd64

```console
$ docker pull jruby@sha256:8944b3e61edc2eed97c1c206aa9f288973adf00a751cc79fd5c06d7ffe312da2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddaa5c279547935447dd77863db5be0a9cfcba5ccf824145d2ccf5e93ad1ffc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 08:46:49 GMT
RUN mkdir -p /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
WORKDIR /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile /usr/src/app/
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile.lock /usr/src/app/
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD RUN bundle install --system
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD ADD . /usr/src/app
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7ce90755a27a64ac75127485786e27a8c7c189ccc6fb2a53fdc58b26baa2a8`  
		Last Modified: Wed, 29 Sep 2021 08:51:35 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jdk`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jdk11`

```console
$ docker pull jruby@sha256:e46f46241a032fdf39a0acffe37e8b6ebff3abc90a9d4b0a0419d5907103673e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:57520b31d3fa224b3f32e19a57e5daf625d36652b92eb7d4fdf33c902a4f848f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.7 MB (363715350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a1cd4436e26b69d2744ea3050990c26598f80cfa81da4a32fae19f5b7d2e6a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:15 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe27974885e6146202139d340f9d214007f05c4fe92ee165893df2fd1349fb`  
		Last Modified: Wed, 29 Sep 2021 08:51:06 GMT  
		Size: 26.4 MB (26356058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f058f16ef05cefa0c10ad38f45972ea136eecd8aa2cfa3c983f2323b24812acf`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f883211ee83ac2b9e6f858dac22726dd0f859a12953f08912af64c7b6a8f4b6`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 1.0 MB (1026802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ba351a88f6273e468ea62357477753f57ba4534d3d022bad2aec4616c4e53`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jdk17`

```console
$ docker pull jruby@sha256:0b338c9487dbb3c483a37b9f88a37f7e151376fb2cd8be930a2eb84e04ff8bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b1374e40da9fe2cd7c6ce4732013681b8a0d0f9fb4588cdaa1d86bc2f58addd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.5 MB (356481056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f1b7a3235d708e688baba164cb95a342fda9b3f1e5e238ac6e6fd62741c94`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:32 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:33 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:42 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:44 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae164902b2e9d3ad535240b63971b8fc137124a8c3538816d4d5233c203e73`  
		Last Modified: Wed, 29 Sep 2021 08:51:22 GMT  
		Size: 26.4 MB (26356030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8520778aaca4506cb538b252ad3893632b13d6814bb57e7747292d8eee722`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe542002860439319b0d002610bd065c7be3dda1db8de9e66b30e4c6a1cce0d`  
		Last Modified: Wed, 29 Sep 2021 08:51:20 GMT  
		Size: 1.0 MB (1026782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc8225ae8eaaa696a6d62f0114b6d4b871a7ddd67940820f205a1317206415`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jdk8`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jre`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jre` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jre11`

```console
$ docker pull jruby@sha256:867ac9cb916f2549a9cc07964cc9e6f23eafca2bd53fbd7bb6e54771f8b5bfed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:94f519a48b6a8eb1118b13f73d05500f9251b62973414e7fa380ac2ad9dd03b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155826436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54fe08f7ef2ea5f938f8eb517261f6b3573de99415ddb5c5a6aaa45d0c2149d`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:56 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:56 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:57 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:07 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:08 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6ba890896c717ec3fc3486f7fc8038cce6c8855b7380ce815e3fcef9e3d9c`  
		Last Modified: Wed, 29 Sep 2021 08:50:51 GMT  
		Size: 26.4 MB (26355822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29610e4a43a92c762d00afdcf506d6772fb88fa09edc9941c4130287daa55a94`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5fa62cd9cfeb7738816def763478d6ebfeaca5b947a5e14759fbf807b23041`  
		Last Modified: Wed, 29 Sep 2021 08:50:49 GMT  
		Size: 1.0 MB (1026797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1760bdc9239d6efc6b23066c8c28f1e7ae9d2cb843ca8bcbf10bf3f278da496d`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-jre8`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2.19-onbuild`

```console
$ docker pull jruby@sha256:4c2a878dc1366a1125ad72dd694e7004fef2e538ef058cc1a0d6274d3c9ba765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2.19-onbuild` - linux; amd64

```console
$ docker pull jruby@sha256:8944b3e61edc2eed97c1c206aa9f288973adf00a751cc79fd5c06d7ffe312da2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddaa5c279547935447dd77863db5be0a9cfcba5ccf824145d2ccf5e93ad1ffc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 08:46:49 GMT
RUN mkdir -p /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
WORKDIR /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile /usr/src/app/
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile.lock /usr/src/app/
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD RUN bundle install --system
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD ADD . /usr/src/app
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7ce90755a27a64ac75127485786e27a8c7c189ccc6fb2a53fdc58b26baa2a8`  
		Last Modified: Wed, 29 Sep 2021 08:51:35 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jdk`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jdk11`

```console
$ docker pull jruby@sha256:e46f46241a032fdf39a0acffe37e8b6ebff3abc90a9d4b0a0419d5907103673e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:57520b31d3fa224b3f32e19a57e5daf625d36652b92eb7d4fdf33c902a4f848f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.7 MB (363715350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a1cd4436e26b69d2744ea3050990c26598f80cfa81da4a32fae19f5b7d2e6a`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:12 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:15 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbe27974885e6146202139d340f9d214007f05c4fe92ee165893df2fd1349fb`  
		Last Modified: Wed, 29 Sep 2021 08:51:06 GMT  
		Size: 26.4 MB (26356058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f058f16ef05cefa0c10ad38f45972ea136eecd8aa2cfa3c983f2323b24812acf`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f883211ee83ac2b9e6f858dac22726dd0f859a12953f08912af64c7b6a8f4b6`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 1.0 MB (1026802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ba351a88f6273e468ea62357477753f57ba4534d3d022bad2aec4616c4e53`  
		Last Modified: Wed, 29 Sep 2021 08:51:04 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jdk17`

```console
$ docker pull jruby@sha256:0b338c9487dbb3c483a37b9f88a37f7e151376fb2cd8be930a2eb84e04ff8bf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b1374e40da9fe2cd7c6ce4732013681b8a0d0f9fb4588cdaa1d86bc2f58addd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.5 MB (356481056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f1b7a3235d708e688baba164cb95a342fda9b3f1e5e238ac6e6fd62741c94`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:46:30 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:46:32 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:46:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:33 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:42 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:43 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:44 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae164902b2e9d3ad535240b63971b8fc137124a8c3538816d4d5233c203e73`  
		Last Modified: Wed, 29 Sep 2021 08:51:22 GMT  
		Size: 26.4 MB (26356030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8520778aaca4506cb538b252ad3893632b13d6814bb57e7747292d8eee722`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe542002860439319b0d002610bd065c7be3dda1db8de9e66b30e4c6a1cce0d`  
		Last Modified: Wed, 29 Sep 2021 08:51:20 GMT  
		Size: 1.0 MB (1026782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc8225ae8eaaa696a6d62f0114b6d4b871a7ddd67940820f205a1317206415`  
		Last Modified: Wed, 29 Sep 2021 08:51:19 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jdk8`

```console
$ docker pull jruby@sha256:a4a12623e45ebd967d68ba9142702763a0ecba6396b33b10ab97562cc0057ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:ab4c742a481e23a97ddb1bbe021a2ad0ad70b429fd94f68a651d378f23707dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5612cde651b5fcac2a12106bec053ed588c615286e4d324bf135e5b4b626e8bc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jre`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jre` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jre11`

```console
$ docker pull jruby@sha256:867ac9cb916f2549a9cc07964cc9e6f23eafca2bd53fbd7bb6e54771f8b5bfed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:94f519a48b6a8eb1118b13f73d05500f9251b62973414e7fa380ac2ad9dd03b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155826436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e54fe08f7ef2ea5f938f8eb517261f6b3573de99415ddb5c5a6aaa45d0c2149d`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:54 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:56 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:56 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:57 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:46:07 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:46:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:46:07 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:46:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:46:08 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6ba890896c717ec3fc3486f7fc8038cce6c8855b7380ce815e3fcef9e3d9c`  
		Last Modified: Wed, 29 Sep 2021 08:50:51 GMT  
		Size: 26.4 MB (26355822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29610e4a43a92c762d00afdcf506d6772fb88fa09edc9941c4130287daa55a94`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5fa62cd9cfeb7738816def763478d6ebfeaca5b947a5e14759fbf807b23041`  
		Last Modified: Wed, 29 Sep 2021 08:50:49 GMT  
		Size: 1.0 MB (1026797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1760bdc9239d6efc6b23066c8c28f1e7ae9d2cb843ca8bcbf10bf3f278da496d`  
		Last Modified: Wed, 29 Sep 2021 08:50:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-jre8`

```console
$ docker pull jruby@sha256:e24f684bcd3b3218eddd4c10f559fd2cfc7de10ee1c0b27524b3140cff39c327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:5d971ef582600ccc9a3b6a6da79241f53ca18cc09d34d84ad54b45481c309627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c3f256a658cd9f62daea7c2459802bd9e27df34e0189d365c3950c8740492c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:16 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:19 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:19 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:20 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:29 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:30 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:31 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c7cc2811bcdf4b70c7cc3b1055440ca7e5d6f677aae8d26b24a76263b2939`  
		Last Modified: Wed, 29 Sep 2021 08:49:50 GMT  
		Size: 26.4 MB (26355934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd1a285e90fa9c41b0351ad5102097eac86d487c9fc726834e9eb80ad394bdf`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ce9f903a1b1ba80e0ae660186c6630238182b0d47bb1ba4ad0b0df68861e54`  
		Last Modified: Wed, 29 Sep 2021 08:49:48 GMT  
		Size: 1.0 MB (1026796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03247c9ff23478042b71a7f425a462aba4bf6875b52c227b693989649b130928`  
		Last Modified: Wed, 29 Sep 2021 08:49:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.2-onbuild`

```console
$ docker pull jruby@sha256:4c2a878dc1366a1125ad72dd694e7004fef2e538ef058cc1a0d6274d3c9ba765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.2-onbuild` - linux; amd64

```console
$ docker pull jruby@sha256:8944b3e61edc2eed97c1c206aa9f288973adf00a751cc79fd5c06d7ffe312da2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.9 MB (270928845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddaa5c279547935447dd77863db5be0a9cfcba5ccf824145d2ccf5e93ad1ffc`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:45:35 GMT
ENV JRUBY_VERSION=9.2.19.0
# Wed, 29 Sep 2021 08:45:36 GMT
ENV JRUBY_SHA256=1f74885a2d3fa589fcbeb292a39facf7f86be3eac1ab015e32c65d32acf3f3bf
# Wed, 29 Sep 2021 08:45:38 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:45:38 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:39 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:48 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:49 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:50 GMT
CMD ["irb"]
# Wed, 29 Sep 2021 08:46:49 GMT
RUN mkdir -p /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
WORKDIR /usr/src/app
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile /usr/src/app/
# Wed, 29 Sep 2021 08:46:49 GMT
ONBUILD ADD Gemfile.lock /usr/src/app/
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD RUN bundle install --system
# Wed, 29 Sep 2021 08:46:50 GMT
ONBUILD ADD . /usr/src/app
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2ecb162f959f1d06821d79a72be2588bfde3f8d258c694da39fbc7957091f`  
		Last Modified: Wed, 29 Sep 2021 08:50:26 GMT  
		Size: 26.4 MB (26356026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5132e39bbec5a601e55d4f961208d64510c2b0fa81fa74564b1df44051dbd5`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfffb193daff58cc17aeb1dce2c9390d4392dad0166448268169e64b102df2e`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 1.0 MB (1026806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee06daedd55285791b10a27e24e15831575b48289b6142724087b0eb1674e90`  
		Last Modified: Wed, 29 Sep 2021 08:50:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7ce90755a27a64ac75127485786e27a8c7c189ccc6fb2a53fdc58b26baa2a8`  
		Last Modified: Wed, 29 Sep 2021 08:51:35 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jdk`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jdk11`

```console
$ docker pull jruby@sha256:1f354bbb1d24c9bdffae32b487d83a82bbdc772799bfed6e7223b7f2e7198610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:5737312f86d6c6cb615f0345d8db88e12fa0256b9da15a5b853fd5fe3e04a7f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.9 MB (364916084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0fe4973a67155cb5b1aed3d24bb902b1109fe87bb0516fded83293e750c7d07`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:33 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:44 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1229213c35390625453a097e042207e1e30b0bffbeaa99f659129ee01f77add`  
		Last Modified: Wed, 29 Sep 2021 08:49:19 GMT  
		Size: 27.6 MB (27556680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28610444109527f385e7f310f4fdca8d50cce49037a907ad75b5aba58db647`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2de67a571a4da417a4128a2d2e9fa67451a77b07164edb17cb72aa5f88a33d5`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 1.0 MB (1026913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfe96c181c270103a8eb873bd613cafb6fd03befc62988232cbcfe8dba7437a`  
		Last Modified: Wed, 29 Sep 2021 08:49:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jdk17`

```console
$ docker pull jruby@sha256:4e55ebf66e86af7ade11ec56b459bcf042216264cc04f9727a47bf45b65626e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:fef18f60b3dc308013623d29cb6ed0cef67d799b234363fb83d5993c35574f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.7 MB (357681917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59746580409f63eb45fa9c129ecfb62d33d725c371e747e3ca5a525884391a9c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:58 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:58 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:59 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:09 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:10 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121c676c8b3899a231a1e8724e9fd4a392905de47580a7c7d0845f7f5e8fee03`  
		Last Modified: Wed, 29 Sep 2021 08:49:34 GMT  
		Size: 27.6 MB (27556785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c63e47de98f093d4de47f3eb3235f0d26cc42bfa671a909a0f33291bd338059`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9220a2f9e9eabdb9136d50a81d7bdb268ca7021d2eb6d76aa53055c333c5cada`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 1.0 MB (1026890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25d1e12d36ffd86e41bf1de5819ca8e1c8ddf80360cfde4fa8c7fa6ccd278ad`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jdk8`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jre`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jre` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jre11`

```console
$ docker pull jruby@sha256:0ae0963b2cd1436fc6236464318d632b39d0011804b995a5c051bee19271855b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:cda501c7adb0278d25a9f4e4a55ee1d33739929d44685680d7a04a8dd5091abb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157027363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44335d61dc90c389ba7dbf423b349b38d03714f830cff889c49c8ed3fdd101f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:08 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:08 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:09 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:19 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:21 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d283c1941e37125a7fa78486b8086e5da1809ce36e32fa823171a39f03f707e9`  
		Last Modified: Wed, 29 Sep 2021 08:49:02 GMT  
		Size: 27.6 MB (27556642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf2f1cbcb4a8814636ce97af8eb4bc1d7cbd7a2a9c4b8eb8875bfc9139002ac`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c159dac84e915468b06ab2b8947b56ba333f089e9eef677652f624ce4a488f`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 1.0 MB (1026903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3522fa355c754596833a03c783bec572954c942f89dd3645d8a2cdcf59df92ee`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0.0-jre8`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0.0-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jdk`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jdk11`

```console
$ docker pull jruby@sha256:1f354bbb1d24c9bdffae32b487d83a82bbdc772799bfed6e7223b7f2e7198610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:5737312f86d6c6cb615f0345d8db88e12fa0256b9da15a5b853fd5fe3e04a7f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.9 MB (364916084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0fe4973a67155cb5b1aed3d24bb902b1109fe87bb0516fded83293e750c7d07`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:33 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:44 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1229213c35390625453a097e042207e1e30b0bffbeaa99f659129ee01f77add`  
		Last Modified: Wed, 29 Sep 2021 08:49:19 GMT  
		Size: 27.6 MB (27556680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28610444109527f385e7f310f4fdca8d50cce49037a907ad75b5aba58db647`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2de67a571a4da417a4128a2d2e9fa67451a77b07164edb17cb72aa5f88a33d5`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 1.0 MB (1026913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfe96c181c270103a8eb873bd613cafb6fd03befc62988232cbcfe8dba7437a`  
		Last Modified: Wed, 29 Sep 2021 08:49:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jdk17`

```console
$ docker pull jruby@sha256:4e55ebf66e86af7ade11ec56b459bcf042216264cc04f9727a47bf45b65626e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:fef18f60b3dc308013623d29cb6ed0cef67d799b234363fb83d5993c35574f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.7 MB (357681917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59746580409f63eb45fa9c129ecfb62d33d725c371e747e3ca5a525884391a9c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:58 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:58 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:59 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:09 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:10 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121c676c8b3899a231a1e8724e9fd4a392905de47580a7c7d0845f7f5e8fee03`  
		Last Modified: Wed, 29 Sep 2021 08:49:34 GMT  
		Size: 27.6 MB (27556785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c63e47de98f093d4de47f3eb3235f0d26cc42bfa671a909a0f33291bd338059`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9220a2f9e9eabdb9136d50a81d7bdb268ca7021d2eb6d76aa53055c333c5cada`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 1.0 MB (1026890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25d1e12d36ffd86e41bf1de5819ca8e1c8ddf80360cfde4fa8c7fa6ccd278ad`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jdk8`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jre`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jre` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jre11`

```console
$ docker pull jruby@sha256:0ae0963b2cd1436fc6236464318d632b39d0011804b995a5c051bee19271855b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:cda501c7adb0278d25a9f4e4a55ee1d33739929d44685680d7a04a8dd5091abb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157027363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44335d61dc90c389ba7dbf423b349b38d03714f830cff889c49c8ed3fdd101f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:08 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:08 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:09 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:19 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:21 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d283c1941e37125a7fa78486b8086e5da1809ce36e32fa823171a39f03f707e9`  
		Last Modified: Wed, 29 Sep 2021 08:49:02 GMT  
		Size: 27.6 MB (27556642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf2f1cbcb4a8814636ce97af8eb4bc1d7cbd7a2a9c4b8eb8875bfc9139002ac`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c159dac84e915468b06ab2b8947b56ba333f089e9eef677652f624ce4a488f`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 1.0 MB (1026903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3522fa355c754596833a03c783bec572954c942f89dd3645d8a2cdcf59df92ee`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.0-jre8`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3.0-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk11`

```console
$ docker pull jruby@sha256:1f354bbb1d24c9bdffae32b487d83a82bbdc772799bfed6e7223b7f2e7198610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:5737312f86d6c6cb615f0345d8db88e12fa0256b9da15a5b853fd5fe3e04a7f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.9 MB (364916084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0fe4973a67155cb5b1aed3d24bb902b1109fe87bb0516fded83293e750c7d07`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:21:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:21:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:21:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:21:24 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:21:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:21:46 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:30 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:30 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:33 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:33 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:44 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:45 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a1491dadda07f29d42317275939f6e75ba1244cded8161cc53918ccb134dc`  
		Last Modified: Tue, 28 Sep 2021 09:43:40 GMT  
		Size: 5.3 MB (5286571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774fbe8201e8b9c341a68f83276fd3a9367c60c569847cb6d8892c6e6c324b83`  
		Last Modified: Tue, 28 Sep 2021 09:43:39 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e27d7befc157e0c423491ee834a20d58ff365e5cde3620eed7b82eb0f841e6`  
		Last Modified: Tue, 28 Sep 2021 09:44:00 GMT  
		Size: 203.1 MB (203129506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd21af714eb26623a6db034709ad82b6838fe40982e71a4b8a9375486a39bf67`  
		Last Modified: Wed, 29 Sep 2021 08:49:18 GMT  
		Size: 7.8 MB (7807488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1229213c35390625453a097e042207e1e30b0bffbeaa99f659129ee01f77add`  
		Last Modified: Wed, 29 Sep 2021 08:49:19 GMT  
		Size: 27.6 MB (27556680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28610444109527f385e7f310f4fdca8d50cce49037a907ad75b5aba58db647`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2de67a571a4da417a4128a2d2e9fa67451a77b07164edb17cb72aa5f88a33d5`  
		Last Modified: Wed, 29 Sep 2021 08:49:17 GMT  
		Size: 1.0 MB (1026913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfe96c181c270103a8eb873bd613cafb6fd03befc62988232cbcfe8dba7437a`  
		Last Modified: Wed, 29 Sep 2021 08:49:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk17`

```console
$ docker pull jruby@sha256:4e55ebf66e86af7ade11ec56b459bcf042216264cc04f9727a47bf45b65626e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:fef18f60b3dc308013623d29cb6ed0cef67d799b234363fb83d5993c35574f6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.7 MB (357681917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59746580409f63eb45fa9c129ecfb62d33d725c371e747e3ca5a525884391a9c`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:14:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:17:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 28 Sep 2021 09:17:09 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:17:09 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:17:09 GMT
ENV JAVA_VERSION=17
# Tue, 28 Sep 2021 09:17:23 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 28 Sep 2021 09:17:24 GMT
CMD ["jshell"]
# Wed, 29 Sep 2021 08:44:55 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:56 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:58 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:58 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:59 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:45:09 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:45:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:45:09 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:45:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:45:10 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f30d24b9c012603ee8c37fa939ed8fe2e353611749561cb1b8dd34f260d5ac`  
		Last Modified: Tue, 28 Sep 2021 09:34:59 GMT  
		Size: 13.9 MB (13921298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258767f01f897aea995e392656b7af7836992eb06303d13516ab0b6a8e43d43`  
		Last Modified: Tue, 28 Sep 2021 09:38:08 GMT  
		Size: 187.3 MB (187259144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f01065669773925d940c9d958aecf63c20669fad66f6921e17c282f54f977a`  
		Last Modified: Wed, 29 Sep 2021 08:49:33 GMT  
		Size: 7.8 MB (7809088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121c676c8b3899a231a1e8724e9fd4a392905de47580a7c7d0845f7f5e8fee03`  
		Last Modified: Wed, 29 Sep 2021 08:49:34 GMT  
		Size: 27.6 MB (27556785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c63e47de98f093d4de47f3eb3235f0d26cc42bfa671a909a0f33291bd338059`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9220a2f9e9eabdb9136d50a81d7bdb268ca7021d2eb6d76aa53055c333c5cada`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 1.0 MB (1026890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25d1e12d36ffd86e41bf1de5819ca8e1c8ddf80360cfde4fa8c7fa6ccd278ad`  
		Last Modified: Wed, 29 Sep 2021 08:49:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk8`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jre` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre11`

```console
$ docker pull jruby@sha256:0ae0963b2cd1436fc6236464318d632b39d0011804b995a5c051bee19271855b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:cda501c7adb0278d25a9f4e4a55ee1d33739929d44685680d7a04a8dd5091abb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157027363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c44335d61dc90c389ba7dbf423b349b38d03714f830cff889c49c8ed3fdd101f`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:23:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 28 Sep 2021 09:23:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:23:53 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:23:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:23:53 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 28 Sep 2021 09:24:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 29 Sep 2021 08:44:05 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:44:05 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:44:08 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:44:08 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:09 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:44:19 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:44:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:44:20 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:44:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:44:21 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed0bec28e48e0638dde134c5468eb83dbb28cc1da758cfebd231f38059bdda1`  
		Last Modified: Tue, 28 Sep 2021 09:45:57 GMT  
		Size: 5.5 MB (5531092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b830dfc52ec401dd9509671b198c59b81326fe4edc6ce36e41e613ec6306d58`  
		Last Modified: Tue, 28 Sep 2021 09:45:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04dffc779e05c2af8a8596b1fb6884fdac4623ddfd15584db1be798380eaac6`  
		Last Modified: Tue, 28 Sep 2021 09:46:05 GMT  
		Size: 46.9 MB (46864161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab61fbac4abc75111ba5580a08badf54d5b2350d85556bfcf7098a4bb53b42`  
		Last Modified: Wed, 29 Sep 2021 08:49:01 GMT  
		Size: 7.8 MB (7780952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d283c1941e37125a7fa78486b8086e5da1809ce36e32fa823171a39f03f707e9`  
		Last Modified: Wed, 29 Sep 2021 08:49:02 GMT  
		Size: 27.6 MB (27556642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf2f1cbcb4a8814636ce97af8eb4bc1d7cbd7a2a9c4b8eb8875bfc9139002ac`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c159dac84e915468b06ab2b8947b56ba333f089e9eef677652f624ce4a488f`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 1.0 MB (1026903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3522fa355c754596833a03c783bec572954c942f89dd3645d8a2cdcf59df92ee`  
		Last Modified: Wed, 29 Sep 2021 08:49:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre8`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9.3-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9-jdk`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9-jdk8`

```console
$ docker pull jruby@sha256:6f477ef0c385f0147f3014b4bd19a156ae79f818fe15db78465f7866a296f23e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:9-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:de2596183010f31a51bca4055579f11486c114b3271c3f5491d5ecb270903508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272129560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b03c2cc104fb6c840e1f0893ea1e4959af0b011cdc38e7572f2921eb3f94235`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:50:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:20:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:24:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:24:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:24:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:24:47 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:24:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:25:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 29 Sep 2021 08:43:39 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:39 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:42 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:52 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:53 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc287cbeddc96a0772397ca00ec85482a7b7f9a9fac643bfddd87b932f743db`  
		Last Modified: Tue, 28 Sep 2021 01:58:12 GMT  
		Size: 54.6 MB (54566880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2961e8351d92060fe0b7d3182dd4725fada0faa44b805531195caf32cb6cc`  
		Last Modified: Tue, 28 Sep 2021 09:42:01 GMT  
		Size: 5.4 MB (5419998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12df774715e16cd39a0150faf0f8a71d1f36c768641e1d731f926d03a6b0f38`  
		Last Modified: Tue, 28 Sep 2021 09:46:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f28107b8b305dfeb6245a285f49bb9b260900c5f8c41a7092796d91ddd6ae8`  
		Last Modified: Tue, 28 Sep 2021 09:46:53 GMT  
		Size: 106.0 MB (105987961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80d40497cf4170682ed5b04a3e133f0c6b9effd7f26d185ff3f2c57dba94759`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 6.6 MB (6617764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8837bd9ce08da2e18140c86ae5032c75fb065d0d8a67d1ca637dcf0ba3b`  
		Last Modified: Wed, 29 Sep 2021 08:48:30 GMT  
		Size: 27.6 MB (27556789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d35a09ffb11ce24c1f43871fa9c68d87a5730edd5b244e4b0f4dddd1c50618a`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdbd3887d9fe7b3e7832fe299f5d5f30086835c35af2daef2aebe970dfb9494`  
		Last Modified: Wed, 29 Sep 2021 08:48:28 GMT  
		Size: 1.0 MB (1026921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1d5382cd4a14ffa18cf2c5c757e74bbd45cf443d3aad17cec365c05e0e4fcd`  
		Last Modified: Wed, 29 Sep 2021 08:48:27 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:latest`

```console
$ docker pull jruby@sha256:8b48540da813ff1134740b2d9fb7b9153a7134c2d1b855dacc58c24faa7b265b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jruby:latest` - linux; amd64

```console
$ docker pull jruby@sha256:a1ac985d3fc813efc8b5c73772f20fede485af7fcfda1d8a2d16e16546c28f70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153142512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7929ede201dc26948b0209798326aa9ab169bb48bc8f536f6ed4de1380b37d4`
-	Default Command: `["irb"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:25 GMT
ADD file:d05a14b1e57f9cc8eeb316a843403bbb35176d6222d60d6ddbb34faba977e316 in / 
# Tue, 28 Sep 2021 01:22:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:49:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 09:22:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:26:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 28 Sep 2021 09:26:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 28 Sep 2021 09:26:49 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Sep 2021 09:26:49 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:26:50 GMT
ENV JAVA_VERSION=8u302
# Tue, 28 Sep 2021 09:27:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 29 Sep 2021 08:43:14 GMT
RUN apt-get update && apt-get install -y libc6-dev --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_VERSION=9.3.0.0
# Wed, 29 Sep 2021 08:43:14 GMT
ENV JRUBY_SHA256=2dc1f85936d3ff3adc20d90e5f4894499c585a7ea5fedec67154e2f9ecb1bc9b
# Wed, 29 Sep 2021 08:43:17 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 29 Sep 2021 08:43:17 GMT
ENV PATH=/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:18 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 29 Sep 2021 08:43:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 29 Sep 2021 08:43:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Sep 2021 08:43:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 08:43:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 29 Sep 2021 08:43:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:df5590a8898bedd76f02205dc8caa5cc9863267dbcd8aac038bcd212688c1cc7`  
		Last Modified: Tue, 28 Sep 2021 01:28:33 GMT  
		Size: 54.9 MB (54927682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705bb4cb554eb7751fd21a994f6f32aee582fbe5ea43037db6c43d321763992b`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 5.2 MB (5153152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519df5fceacdeaadeec563397b1d9f4d7c29c9f6eff879739cab6f0c144f49e1`  
		Last Modified: Tue, 28 Sep 2021 01:57:51 GMT  
		Size: 10.9 MB (10871798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc850b11e97cfdecca53799a94b78db748c40ae0a76694dbc10af9cd746c1229`  
		Last Modified: Tue, 28 Sep 2021 09:45:06 GMT  
		Size: 5.7 MB (5653948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68accb5562eba4dd2f73905ccaf67ad60e40faaabc20f8fb573e9bb2d76197dc`  
		Last Modified: Tue, 28 Sep 2021 09:48:40 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ddc9323ff0ff81badeca7b50ad1e0986157ffad2874d4cf6ba29a73ac82cf`  
		Last Modified: Tue, 28 Sep 2021 09:48:47 GMT  
		Size: 41.4 MB (41358587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38baac085287ce134d99fd7b1752162acb7c8e06a2b5a72dab1358b20612a27d`  
		Last Modified: Wed, 29 Sep 2021 08:47:48 GMT  
		Size: 6.6 MB (6593121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac09556ce91717c2300cf84d78f47afc149ae4674667c56ebb9607e67aa754c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:49 GMT  
		Size: 27.6 MB (27556697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3d5d482d5c0849e16f5909ffe89e0647c93e4612e4ba89d3320b72ee7b7f7`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9606e66bb754ca836903f0cf47e66e4c2217cd2f70b972dd18f8995f43271560`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 1.0 MB (1026915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0e7936da52bd3c5e6c61121385de55d0e6bb78da023c8f56b9e6de8d7690c8`  
		Last Modified: Wed, 29 Sep 2021 08:47:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
