<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `lightstreamer`

-	[`lightstreamer:6`](#lightstreamer6)
-	[`lightstreamer:6.0`](#lightstreamer60)
-	[`lightstreamer:6.0.3`](#lightstreamer603)
-	[`lightstreamer:6.1`](#lightstreamer61)
-	[`lightstreamer:6.1.0`](#lightstreamer610)
-	[`lightstreamer:7-jdk11`](#lightstreamer7-jdk11)
-	[`lightstreamer:7-jdk11-openjdk`](#lightstreamer7-jdk11-openjdk)
-	[`lightstreamer:7-jdk8`](#lightstreamer7-jdk8)
-	[`lightstreamer:7-jdk8-openjdk`](#lightstreamer7-jdk8-openjdk)
-	[`lightstreamer:7.0`](#lightstreamer70)
-	[`lightstreamer:7.0-jdk11`](#lightstreamer70-jdk11)
-	[`lightstreamer:7.0-jdk11-openjdk`](#lightstreamer70-jdk11-openjdk)
-	[`lightstreamer:7.0-jdk8`](#lightstreamer70-jdk8)
-	[`lightstreamer:7.0-jdk8-openjdk`](#lightstreamer70-jdk8-openjdk)
-	[`lightstreamer:7.0.3`](#lightstreamer703)
-	[`lightstreamer:7.0.3-jdk11`](#lightstreamer703-jdk11)
-	[`lightstreamer:7.0.3-jdk11-openjdk`](#lightstreamer703-jdk11-openjdk)
-	[`lightstreamer:7.0.3-jdk8`](#lightstreamer703-jdk8)
-	[`lightstreamer:7.0.3-jdk8-openjdk`](#lightstreamer703-jdk8-openjdk)
-	[`lightstreamer:7.1`](#lightstreamer71)
-	[`lightstreamer:7.1-jdk11`](#lightstreamer71-jdk11)
-	[`lightstreamer:7.1-jdk11-openjdk`](#lightstreamer71-jdk11-openjdk)
-	[`lightstreamer:7.1-jdk8`](#lightstreamer71-jdk8)
-	[`lightstreamer:7.1-jdk8-openjdk`](#lightstreamer71-jdk8-openjdk)
-	[`lightstreamer:7.1.3`](#lightstreamer713)
-	[`lightstreamer:7.1.3-jdk11`](#lightstreamer713-jdk11)
-	[`lightstreamer:7.1.3-jdk11-openjdk`](#lightstreamer713-jdk11-openjdk)
-	[`lightstreamer:7.1.3-jdk8`](#lightstreamer713-jdk8)
-	[`lightstreamer:7.1.3-jdk8-openjdk`](#lightstreamer713-jdk8-openjdk)
-	[`lightstreamer:7.2`](#lightstreamer72)
-	[`lightstreamer:7.2-jd8-openjdk`](#lightstreamer72-jd8-openjdk)
-	[`lightstreamer:7.2-jdk11`](#lightstreamer72-jdk11)
-	[`lightstreamer:7.2-jdk11-openjdk`](#lightstreamer72-jdk11-openjdk)
-	[`lightstreamer:7.2-jdk8`](#lightstreamer72-jdk8)
-	[`lightstreamer:7.2.2`](#lightstreamer722)
-	[`lightstreamer:7.2.2-jdk11`](#lightstreamer722-jdk11)
-	[`lightstreamer:7.2.2-jdk11-openjdk`](#lightstreamer722-jdk11-openjdk)
-	[`lightstreamer:7.2.2-jdk8`](#lightstreamer722-jdk8)
-	[`lightstreamer:7.2.2-jdk8-openjdk`](#lightstreamer722-jdk8-openjdk)
-	[`lightstreamer:latest`](#lightstreamerlatest)

## `lightstreamer:6`

```console
$ docker pull lightstreamer@sha256:0ab7b1d0040cfd1e9006fc1702b2303ea0f19d489679453405e81a4c901f99bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1c7fc83a35a8e77f1f675664501b3879285a1a72e0c3fea1f66ca429fa9b14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273520830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf263d8d19110b8cdfb28d452e1adbcd83b5b185a4a11ef95ec6aedecbfc0d2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:19:55 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:20:31 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Fri, 04 Feb 2022 00:20:53 GMT
WORKDIR /lightstreamer
# Fri, 04 Feb 2022 00:21:03 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Fri, 04 Feb 2022 00:21:04 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:04 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:04 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130abd28ef2c816d02d6fbb7466d2238f030cb8299442da742d38fa695b46803`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a380901fa5305e3460702fa286d78b5eb4b0e6e06993a1309fbee3a696c627b3`  
		Last Modified: Fri, 04 Feb 2022 00:23:42 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abce22242d3b8a7fb29acebe046955cfd13a73bb7cb6693f4bc5d9bb78d20ee`  
		Last Modified: Fri, 04 Feb 2022 00:23:46 GMT  
		Size: 36.5 MB (36516642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.0`

```console
$ docker pull lightstreamer@sha256:d19b671583966e57e4cabd946245d5c1d72b5f29e80d860bc125562c065af675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e3b7b9fa9d5108faecc7a344c62cc70dd7b572d6bb56b0819119b5400bcdcc4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274799557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a441042fa26cddba564a431ef61b4be3127e2546d59843f2e7d1a01d9fcad5e`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:19:55 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:20:31 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_VERSION=6_0_3_20160905
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_0_3_20160905.tar.gz
# Fri, 04 Feb 2022 00:20:32 GMT
WORKDIR /lightstreamer
# Fri, 04 Feb 2022 00:20:43 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Fri, 04 Feb 2022 00:20:43 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:20:43 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:20:44 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130abd28ef2c816d02d6fbb7466d2238f030cb8299442da742d38fa695b46803`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97459a7c92510d9f144273a8ee28f2c3dde126b553136ccd201682c94dab8e6`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0b39bff05d5b7ce079cb86f076907285e47c0cf658b36a3ba3fcd216efc6c1`  
		Last Modified: Fri, 04 Feb 2022 00:23:33 GMT  
		Size: 37.8 MB (37795369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.0.3`

```console
$ docker pull lightstreamer@sha256:d19b671583966e57e4cabd946245d5c1d72b5f29e80d860bc125562c065af675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.0.3` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e3b7b9fa9d5108faecc7a344c62cc70dd7b572d6bb56b0819119b5400bcdcc4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274799557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a441042fa26cddba564a431ef61b4be3127e2546d59843f2e7d1a01d9fcad5e`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:19:55 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:20:31 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_VERSION=6_0_3_20160905
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_0_3_20160905.tar.gz
# Fri, 04 Feb 2022 00:20:32 GMT
WORKDIR /lightstreamer
# Fri, 04 Feb 2022 00:20:43 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Fri, 04 Feb 2022 00:20:43 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:20:43 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:20:44 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130abd28ef2c816d02d6fbb7466d2238f030cb8299442da742d38fa695b46803`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97459a7c92510d9f144273a8ee28f2c3dde126b553136ccd201682c94dab8e6`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0b39bff05d5b7ce079cb86f076907285e47c0cf658b36a3ba3fcd216efc6c1`  
		Last Modified: Fri, 04 Feb 2022 00:23:33 GMT  
		Size: 37.8 MB (37795369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.1`

```console
$ docker pull lightstreamer@sha256:0ab7b1d0040cfd1e9006fc1702b2303ea0f19d489679453405e81a4c901f99bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.1` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1c7fc83a35a8e77f1f675664501b3879285a1a72e0c3fea1f66ca429fa9b14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273520830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf263d8d19110b8cdfb28d452e1adbcd83b5b185a4a11ef95ec6aedecbfc0d2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:19:55 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:20:31 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Fri, 04 Feb 2022 00:20:53 GMT
WORKDIR /lightstreamer
# Fri, 04 Feb 2022 00:21:03 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Fri, 04 Feb 2022 00:21:04 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:04 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:04 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130abd28ef2c816d02d6fbb7466d2238f030cb8299442da742d38fa695b46803`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a380901fa5305e3460702fa286d78b5eb4b0e6e06993a1309fbee3a696c627b3`  
		Last Modified: Fri, 04 Feb 2022 00:23:42 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abce22242d3b8a7fb29acebe046955cfd13a73bb7cb6693f4bc5d9bb78d20ee`  
		Last Modified: Fri, 04 Feb 2022 00:23:46 GMT  
		Size: 36.5 MB (36516642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.1.0`

```console
$ docker pull lightstreamer@sha256:0ab7b1d0040cfd1e9006fc1702b2303ea0f19d489679453405e81a4c901f99bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.1.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1c7fc83a35a8e77f1f675664501b3879285a1a72e0c3fea1f66ca429fa9b14b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273520830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf263d8d19110b8cdfb28d452e1adbcd83b5b185a4a11ef95ec6aedecbfc0d2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:19:55 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:20:31 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:20:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Fri, 04 Feb 2022 00:20:53 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Fri, 04 Feb 2022 00:20:53 GMT
WORKDIR /lightstreamer
# Fri, 04 Feb 2022 00:21:03 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Fri, 04 Feb 2022 00:21:04 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:04 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:04 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130abd28ef2c816d02d6fbb7466d2238f030cb8299442da742d38fa695b46803`  
		Last Modified: Fri, 04 Feb 2022 00:23:29 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a380901fa5305e3460702fa286d78b5eb4b0e6e06993a1309fbee3a696c627b3`  
		Last Modified: Fri, 04 Feb 2022 00:23:42 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abce22242d3b8a7fb29acebe046955cfd13a73bb7cb6693f4bc5d9bb78d20ee`  
		Last Modified: Fri, 04 Feb 2022 00:23:46 GMT  
		Size: 36.5 MB (36516642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk11`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk8`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk11`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk8`

```console
$ docker pull lightstreamer@sha256:2b8c9b76bfb99df1a932831c728721ee2ff97770314ae5b0a5c3e3e52af705e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:6c34d782bb8743d902d6b199d2dd06a9b635d8900f3cdea0ed044b1664ffdf45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270460077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7e25b2410c674814c94547845af8e2f8c21f377af50914dd891c28252f4805`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:21:23 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Fri, 04 Feb 2022 00:21:34 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:21:34 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:21:34 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:34 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:35 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90ff51b9bd45326a283f21a70e831c31113f4dac5a559e9911dc2c678133260`  
		Last Modified: Fri, 04 Feb 2022 00:23:58 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea10998b25390157255e0cedd95a4b578e883ffd33dcdfd3fc9ba4f43211c10`  
		Last Modified: Fri, 04 Feb 2022 00:24:00 GMT  
		Size: 33.5 MB (33456024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:2b8c9b76bfb99df1a932831c728721ee2ff97770314ae5b0a5c3e3e52af705e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:6c34d782bb8743d902d6b199d2dd06a9b635d8900f3cdea0ed044b1664ffdf45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270460077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7e25b2410c674814c94547845af8e2f8c21f377af50914dd891c28252f4805`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:21:23 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Fri, 04 Feb 2022 00:21:34 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:21:34 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:21:34 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:34 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:35 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90ff51b9bd45326a283f21a70e831c31113f4dac5a559e9911dc2c678133260`  
		Last Modified: Fri, 04 Feb 2022 00:23:58 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea10998b25390157255e0cedd95a4b578e883ffd33dcdfd3fc9ba4f43211c10`  
		Last Modified: Fri, 04 Feb 2022 00:24:00 GMT  
		Size: 33.5 MB (33456024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk11`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:d0a7dd7a1626f604cff519bcc9839ef05ea705d0f5dec6d30e21bf50d3037fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:26ee2de07e2476ec1dc5564f21879c0bf2a6d754ad76f602fb4c99e52999517f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367641304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2df7c6b26070b6cea7a213b09e85513a4b4a1c641950d15588e626a64714baeb`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:01 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 04:34:01 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 04:34:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:34:17 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:34:17 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:34:18 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:34:18 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c54913ac36a741a817677e4a79ff101872db73bbde5468603d62b394ccea79`  
		Last Modified: Sat, 12 Feb 2022 04:36:33 GMT  
		Size: 2.4 KB (2409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c99e3b35381ab3734bab8992d2dcd3690fdd452be93da0545e893f15b73a7`  
		Last Modified: Sat, 12 Feb 2022 04:36:35 GMT  
		Size: 33.5 MB (33456098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:7ec1b3037de03e11a054bb6899c654208c83162c4bf2c1d624e3bea607b6e4ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.8 MB (363836868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11591e4c4663b769f849e54a7c6075317b5ff1cd4078483acc421755f51bbf75`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:06:19 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:06:20 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Sat, 12 Feb 2022 02:06:21 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Sat, 12 Feb 2022 02:06:37 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:06:38 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:06:38 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:06:39 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:06:40 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939cb2fac531057ea07c6e0e76b9e900ae61a11a5c5ddb554635c9a2d29a3470`  
		Last Modified: Sat, 12 Feb 2022 02:09:55 GMT  
		Size: 2.4 KB (2381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f219bbcd327762e81a281e3d9a26092a639c055a6e42d81b2e5542c1729998`  
		Last Modified: Sat, 12 Feb 2022 02:09:58 GMT  
		Size: 33.5 MB (33455870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk8`

```console
$ docker pull lightstreamer@sha256:2b8c9b76bfb99df1a932831c728721ee2ff97770314ae5b0a5c3e3e52af705e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0.3-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:6c34d782bb8743d902d6b199d2dd06a9b635d8900f3cdea0ed044b1664ffdf45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270460077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7e25b2410c674814c94547845af8e2f8c21f377af50914dd891c28252f4805`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:21:23 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Fri, 04 Feb 2022 00:21:34 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:21:34 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:21:34 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:34 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:35 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90ff51b9bd45326a283f21a70e831c31113f4dac5a559e9911dc2c678133260`  
		Last Modified: Fri, 04 Feb 2022 00:23:58 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea10998b25390157255e0cedd95a4b578e883ffd33dcdfd3fc9ba4f43211c10`  
		Last Modified: Fri, 04 Feb 2022 00:24:00 GMT  
		Size: 33.5 MB (33456024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:2b8c9b76bfb99df1a932831c728721ee2ff97770314ae5b0a5c3e3e52af705e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0.3-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:6c34d782bb8743d902d6b199d2dd06a9b635d8900f3cdea0ed044b1664ffdf45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.5 MB (270460077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7e25b2410c674814c94547845af8e2f8c21f377af50914dd891c28252f4805`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:21:23 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Fri, 04 Feb 2022 00:21:24 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Fri, 04 Feb 2022 00:21:34 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:21:34 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:21:34 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:21:34 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:21:35 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90ff51b9bd45326a283f21a70e831c31113f4dac5a559e9911dc2c678133260`  
		Last Modified: Fri, 04 Feb 2022 00:23:58 GMT  
		Size: 2.4 KB (2410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea10998b25390157255e0cedd95a4b578e883ffd33dcdfd3fc9ba4f43211c10`  
		Last Modified: Fri, 04 Feb 2022 00:24:00 GMT  
		Size: 33.5 MB (33456024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk11`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk8`

```console
$ docker pull lightstreamer@sha256:311f97c7405ee159dc6d503762e977b0025353ea838e14c1d29daed9ffc4f5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e7954dcd18e90c2380015cbfc35596e0891dae6268d6668d296ec59205358ff6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.1 MB (287076566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9688680d2fa5c2e6a82b4718c89844fe5e4426c05851238dd16dcd5e07bcc60f`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Fri, 04 Feb 2022 00:22:13 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:14 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:14 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:14 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:14 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48459bb30bac31b43516318341cdad3a56a273ab1ae053ebaf19724320d972c`  
		Last Modified: Fri, 04 Feb 2022 00:24:41 GMT  
		Size: 50.1 MB (50072517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:311f97c7405ee159dc6d503762e977b0025353ea838e14c1d29daed9ffc4f5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e7954dcd18e90c2380015cbfc35596e0891dae6268d6668d296ec59205358ff6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.1 MB (287076566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9688680d2fa5c2e6a82b4718c89844fe5e4426c05851238dd16dcd5e07bcc60f`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Fri, 04 Feb 2022 00:22:13 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:14 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:14 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:14 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:14 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48459bb30bac31b43516318341cdad3a56a273ab1ae053ebaf19724320d972c`  
		Last Modified: Fri, 04 Feb 2022 00:24:41 GMT  
		Size: 50.1 MB (50072517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.3`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.3` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.3` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.3-jdk11`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.3-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.3-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.3-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:e4b1f18ab4a05758a3184ce197055eb6831f4b95f87b3181a894e67fdafba7fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.3-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:9e98d212f4739de658e94e82bd4fe86f5dcc34596feb3e7d62683bb19e8c788b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.3 MB (384257697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c087b59789a5f5a5de9f6c5942231af66d11c753cb8b361ef91aa57a50897ffd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 04:34:57 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 04:35:24 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:24 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:25 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:25 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b0a56b577be3d3c98e46b5ce436b160302f79dd86c9905328e36912c83630`  
		Last Modified: Sat, 12 Feb 2022 04:37:00 GMT  
		Size: 50.1 MB (50072494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.3-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:98940f28d0efefbf061a1410836c5397113df68baa56fba6e90325f70179b281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380453325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97590e300f4ab99c97ae409f57ca4e87b231954f1a03ef19bd34d2900478e0c5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:07:36 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Sat, 12 Feb 2022 02:07:37 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Sat, 12 Feb 2022 02:07:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Sat, 12 Feb 2022 02:08:07 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:08 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:08 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:09 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:10 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e50f442f6473dc5c52328db0027028536e7f524c87b1d1220d85edb54dc0c4`  
		Last Modified: Sat, 12 Feb 2022 02:10:27 GMT  
		Size: 50.1 MB (50072332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.3-jdk8`

```console
$ docker pull lightstreamer@sha256:311f97c7405ee159dc6d503762e977b0025353ea838e14c1d29daed9ffc4f5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1.3-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e7954dcd18e90c2380015cbfc35596e0891dae6268d6668d296ec59205358ff6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.1 MB (287076566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9688680d2fa5c2e6a82b4718c89844fe5e4426c05851238dd16dcd5e07bcc60f`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Fri, 04 Feb 2022 00:22:13 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:14 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:14 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:14 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:14 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48459bb30bac31b43516318341cdad3a56a273ab1ae053ebaf19724320d972c`  
		Last Modified: Fri, 04 Feb 2022 00:24:41 GMT  
		Size: 50.1 MB (50072517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.3-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:311f97c7405ee159dc6d503762e977b0025353ea838e14c1d29daed9ffc4f5f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1.3-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e7954dcd18e90c2380015cbfc35596e0891dae6268d6668d296ec59205358ff6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.1 MB (287076566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9688680d2fa5c2e6a82b4718c89844fe5e4426c05851238dd16dcd5e07bcc60f`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_VERSION=7_1_3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_FOLDER=7.1.3
# Fri, 04 Feb 2022 00:22:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.1.3/Lightstreamer_7_1_3.tar.gz
# Fri, 04 Feb 2022 00:22:13 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:14 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:14 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:14 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:14 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48459bb30bac31b43516318341cdad3a56a273ab1ae053ebaf19724320d972c`  
		Last Modified: Fri, 04 Feb 2022 00:24:41 GMT  
		Size: 50.1 MB (50072517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jd8-openjdk`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jd8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jd8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk11`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk8`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.2`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.2` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.2` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.2-jdk11`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.2-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.2-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.2-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.2-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.2-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.2-jdk8`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.2-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.2-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.2-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:89bb2ce43a321e49fd29658e97ba00ba645c8da7bd381489500dc62fb41b25b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.2-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ea8b71036081101a493a38a9e4db888251d1189629dd969aae828efae0f784e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.9 MB (286855240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90df3508b3deafdea55de5c2b410414682709821e138a166bfac267b374f67de`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:29:49 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 09:29:50 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:29:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:29:50 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:46:19 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:46:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:21:07 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:22:04 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:22:41 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:22:44 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:22:44 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:22:45 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:22:45 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:22:45 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b5bcea956cbbcc7e16356354d5eb4b5b3834a43d708ca6c3fd048f33ddc579`  
		Last Modified: Wed, 26 Jan 2022 09:55:46 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed70148ebcf78cba8546f5af3e152a6d9422a3a9d814d7683242e4663e773c3`  
		Last Modified: Thu, 03 Feb 2022 21:02:59 GMT  
		Size: 106.1 MB (106072294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e7e11d64ee7900715df389d666fd0ce1018bac362da7e119eb76eaa15800c1`  
		Last Modified: Fri, 04 Feb 2022 00:24:38 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb75f5abbe5f77c67912ad674d61150bd3ac2de4e838a9da6c226f1887b00b`  
		Last Modified: Fri, 04 Feb 2022 00:25:56 GMT  
		Size: 49.9 MB (49851191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.2-jdk8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:a0f28b3dfbf41b4a4c1be15da1052347b73361d2115141e0450eeb97f5af5f65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284435828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca5d475cbd532015f6584ce11752706959c5dfe9d83edaf5c18e7c1f58719535`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:00:48 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:49 GMT
ENV LANG=C.UTF-8
# Thu, 03 Feb 2022 20:57:54 GMT
ENV JAVA_VERSION=8u322
# Thu, 03 Feb 2022 20:58:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 04 Feb 2022 00:33:08 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Fri, 04 Feb 2022 00:33:41 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Fri, 04 Feb 2022 00:33:41 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Fri, 04 Feb 2022 00:33:42 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Fri, 04 Feb 2022 00:33:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Fri, 04 Feb 2022 00:33:46 GMT
USER lightstreamer
# Fri, 04 Feb 2022 00:33:47 GMT
EXPOSE 8080
# Fri, 04 Feb 2022 00:33:48 GMT
WORKDIR /lightstreamer/bin/unix-like
# Fri, 04 Feb 2022 00:33:49 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3973acc73ccb4db4685136c67eb73dd02f02b1518d5381cf376d82710758caa`  
		Last Modified: Wed, 26 Jan 2022 06:28:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7bbf4c253ea3a60b3244eff075f853bbc379581d997b227a597daba7382ba`  
		Last Modified: Thu, 03 Feb 2022 21:18:22 GMT  
		Size: 105.1 MB (105086380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88a83e2c0b8ec6134a12245bfc3b91c4b69e3d257affb85b35f5fc1fd91b3c2`  
		Last Modified: Fri, 04 Feb 2022 00:36:23 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62e0437522ed44acf8d6ec93c5a50521e9bffe15dcc737212e980d4369fe5cc`  
		Last Modified: Fri, 04 Feb 2022 00:36:28 GMT  
		Size: 49.9 MB (49850899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:latest`

```console
$ docker pull lightstreamer@sha256:3b2c777c3d3d9a4c7d07cc7701808b1cfe87f993a34e9f00e4ae1a1f3983a9ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:latest` - linux; amd64

```console
$ docker pull lightstreamer@sha256:4e7c2515355a01d1a6c70144333b71248219ce051108e02ff4551d304c8b7df1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384036402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878d3f965a8c68ac2d78f862959e7fdc15d09742826c9bcad1c69263a10d4c89`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:24:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 09:24:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 09:24:14 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:24:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:57:23 GMT
ENV JAVA_VERSION=11.0.14.1
# Fri, 11 Feb 2022 23:57:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:57:59 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 04:33:29 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 04:34:57 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 04:35:37 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 04:35:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 04:35:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 04:35:46 GMT
USER lightstreamer
# Sat, 12 Feb 2022 04:35:46 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 04:35:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 04:35:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461bb1d8c517c7f9fc0f1df66c9dc34c85a23421c1e1c540b2e28cbb258e75f5`  
		Last Modified: Wed, 26 Jan 2022 02:22:32 GMT  
		Size: 54.6 MB (54567492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e442ee9d8dd9896a5b3b67117060f2af4ae8e997af7297009e7d0ea4b6595163`  
		Last Modified: Wed, 26 Jan 2022 09:50:58 GMT  
		Size: 5.4 MB (5420014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c9fe4a7ba162c9efa211454e660394ae5b686c315a05b000b985ff6d8786b`  
		Last Modified: Wed, 26 Jan 2022 09:50:57 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41de18d1833d2d5e6cb6111780577f3eab0afd9b1bf6c0c1756c5227abfa645c`  
		Last Modified: Sat, 12 Feb 2022 00:21:20 GMT  
		Size: 203.3 MB (203253446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a1d66d62a831d87b4554a6197ce54e113baceda6c9d385d11623fbfc23e59`  
		Last Modified: Sat, 12 Feb 2022 04:36:57 GMT  
		Size: 2.4 KB (2406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614688d9556abb5e291f41041556857085f51ec7db5977fa3871bb7c2a114e6e`  
		Last Modified: Sat, 12 Feb 2022 04:37:24 GMT  
		Size: 49.9 MB (49851199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:latest` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:2c69e16c9712ed8f2e17e3c0be27aa79bd834444297690d1f08bff3e8091cfaf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.2 MB (380231878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb6c9cf7b1064a0ba75bfcd14ba42c2d776eb47eacfb2983c173ff0f2f9b107`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:56:07 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 05:56:08 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 05:56:09 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:56:10 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:14:16 GMT
ENV JAVA_VERSION=11.0.14.1
# Sat, 12 Feb 2022 00:14:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_11.0.14.1_1.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_11.0.14.1_1.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:14:30 GMT
CMD ["jshell"]
# Sat, 12 Feb 2022 02:05:43 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Sat, 12 Feb 2022 02:07:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Sat, 12 Feb 2022 02:08:22 GMT
ENV LIGHTSTREAMER_VERSION=7.2.2
# Sat, 12 Feb 2022 02:08:23 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://lightstreamer.com/distr/ls-server/7.2.2/Lightstreamer-7.2.2.tar.gz
# Sat, 12 Feb 2022 02:08:48 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Sat, 12 Feb 2022 02:08:48 GMT
USER lightstreamer
# Sat, 12 Feb 2022 02:08:49 GMT
EXPOSE 8080
# Sat, 12 Feb 2022 02:08:50 GMT
WORKDIR /lightstreamer/bin/unix-like
# Sat, 12 Feb 2022 02:08:51 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f1769d50d3693321e1b48f527d9c920830ad24d931b642c116bf7823bed6a`  
		Last Modified: Wed, 26 Jan 2022 02:24:10 GMT  
		Size: 54.7 MB (54669460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5cb8edd8beada37ea034ed391c47dfd106ff9cc9fac852e0f52db0b063374f`  
		Last Modified: Wed, 26 Jan 2022 06:23:05 GMT  
		Size: 5.4 MB (5420184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9ec958687a4a0b67ab7f3a7528f4f1945a08921290b7dfc26c085083f85b2d`  
		Last Modified: Wed, 26 Jan 2022 06:23:04 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0808bac692f89cb535b2bb3c119ebe9ce5b3015fcefab3bb87d42ff83cdaad5c`  
		Last Modified: Sat, 12 Feb 2022 00:40:39 GMT  
		Size: 200.9 MB (200882444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798c002cce314d837d83a905a03c3e89a2ab523a2e7f9b31cc54930618f65c1d`  
		Last Modified: Sat, 12 Feb 2022 02:10:22 GMT  
		Size: 2.4 KB (2376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815f77fcc766d4633f27d1f940c37d33fd98ea8187fe8f2196690a01aac030c1`  
		Last Modified: Sat, 12 Feb 2022 02:10:55 GMT  
		Size: 49.9 MB (49850885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
