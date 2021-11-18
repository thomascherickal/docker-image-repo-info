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
-	[`lightstreamer:7.1.2`](#lightstreamer712)
-	[`lightstreamer:7.1.2-jdk11`](#lightstreamer712-jdk11)
-	[`lightstreamer:7.1.2-jdk11-openjdk`](#lightstreamer712-jdk11-openjdk)
-	[`lightstreamer:7.1.2-jdk8`](#lightstreamer712-jdk8)
-	[`lightstreamer:7.1.2-jdk8-openjdk`](#lightstreamer712-jdk8-openjdk)
-	[`lightstreamer:7.2`](#lightstreamer72)
-	[`lightstreamer:7.2-jd8-openjdk`](#lightstreamer72-jd8-openjdk)
-	[`lightstreamer:7.2-jdk11`](#lightstreamer72-jdk11)
-	[`lightstreamer:7.2-jdk11-openjdk`](#lightstreamer72-jdk11-openjdk)
-	[`lightstreamer:7.2-jdk8`](#lightstreamer72-jdk8)
-	[`lightstreamer:7.2.0`](#lightstreamer720)
-	[`lightstreamer:7.2.0-jdk11`](#lightstreamer720-jdk11)
-	[`lightstreamer:7.2.0-jdk11-openjdk`](#lightstreamer720-jdk11-openjdk)
-	[`lightstreamer:7.2.0-jdk8`](#lightstreamer720-jdk8)
-	[`lightstreamer:7.2.0-jdk8-openjdk`](#lightstreamer720-jdk8-openjdk)
-	[`lightstreamer:latest`](#lightstreamerlatest)

## `lightstreamer:6`

```console
$ docker pull lightstreamer@sha256:d817c4f9d46352fc9f311e929c8a50744c999e8ee9b3588b61ff48d037c8e7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1ad2a23fc88f4a10c96bb7b657ee5653b57f2758cc038aa6ceeb7eb281ee7cab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273462933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55a0c8dd58923ae8ddc551cd8cf574bdc83518ad0d577adf541c99d2e453808`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:07:21 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:07:32 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Thu, 18 Nov 2021 11:07:48 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Thu, 18 Nov 2021 11:07:49 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Thu, 18 Nov 2021 11:07:49 GMT
WORKDIR /lightstreamer
# Thu, 18 Nov 2021 11:07:59 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Thu, 18 Nov 2021 11:07:59 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:00 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:00 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328f508a7a13aec2494ba929c34edde250cc8ed239e0764f0d8df13fd1521c5`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d141a8b552c80abb6862a627de1d3a7e29e0db42ba01078556e0038443432d2e`  
		Last Modified: Thu, 18 Nov 2021 11:10:46 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3445573f7f6254b2ba9e0154b0ec694a5371151d5a479bd86df27f0db054fa`  
		Last Modified: Thu, 18 Nov 2021 11:10:50 GMT  
		Size: 36.5 MB (36516832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.0`

```console
$ docker pull lightstreamer@sha256:38d363f5efc381dd0708585334d9b7024946079b127559ac67979048eeb539e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e0df69be002a5c72925461b22d6cf9413d3597230397fb8ecdb0bd4c14d1f090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274741482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f1293bba201db749e3b3776d053e01c7181f4adaa3a423b8fa846233ddc553`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:07:21 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:07:32 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_VERSION=6_0_3_20160905
# Thu, 18 Nov 2021 11:07:33 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_0_3_20160905.tar.gz
# Thu, 18 Nov 2021 11:07:33 GMT
WORKDIR /lightstreamer
# Thu, 18 Nov 2021 11:07:45 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Thu, 18 Nov 2021 11:07:46 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:07:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:07:46 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328f508a7a13aec2494ba929c34edde250cc8ed239e0764f0d8df13fd1521c5`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1cfc51b6f8204be71502b4104f8e6b013c757952b8f9912fcd153104cfd1fc`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd124185d31abd3ef1b8310222bdf5e11f8e66a925ccee0f281816f81c899a37`  
		Last Modified: Thu, 18 Nov 2021 11:10:37 GMT  
		Size: 37.8 MB (37795381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.0.3`

```console
$ docker pull lightstreamer@sha256:38d363f5efc381dd0708585334d9b7024946079b127559ac67979048eeb539e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.0.3` - linux; amd64

```console
$ docker pull lightstreamer@sha256:e0df69be002a5c72925461b22d6cf9413d3597230397fb8ecdb0bd4c14d1f090
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274741482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f1293bba201db749e3b3776d053e01c7181f4adaa3a423b8fa846233ddc553`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:07:21 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:07:32 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_VERSION=6_0_3_20160905
# Thu, 18 Nov 2021 11:07:33 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_0_3_20160905.tar.gz
# Thu, 18 Nov 2021 11:07:33 GMT
WORKDIR /lightstreamer
# Thu, 18 Nov 2021 11:07:45 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Thu, 18 Nov 2021 11:07:46 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:07:46 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:07:46 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328f508a7a13aec2494ba929c34edde250cc8ed239e0764f0d8df13fd1521c5`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1cfc51b6f8204be71502b4104f8e6b013c757952b8f9912fcd153104cfd1fc`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd124185d31abd3ef1b8310222bdf5e11f8e66a925ccee0f281816f81c899a37`  
		Last Modified: Thu, 18 Nov 2021 11:10:37 GMT  
		Size: 37.8 MB (37795381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.1`

```console
$ docker pull lightstreamer@sha256:d817c4f9d46352fc9f311e929c8a50744c999e8ee9b3588b61ff48d037c8e7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.1` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1ad2a23fc88f4a10c96bb7b657ee5653b57f2758cc038aa6ceeb7eb281ee7cab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273462933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55a0c8dd58923ae8ddc551cd8cf574bdc83518ad0d577adf541c99d2e453808`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:07:21 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:07:32 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Thu, 18 Nov 2021 11:07:48 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Thu, 18 Nov 2021 11:07:49 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Thu, 18 Nov 2021 11:07:49 GMT
WORKDIR /lightstreamer
# Thu, 18 Nov 2021 11:07:59 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Thu, 18 Nov 2021 11:07:59 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:00 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:00 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328f508a7a13aec2494ba929c34edde250cc8ed239e0764f0d8df13fd1521c5`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d141a8b552c80abb6862a627de1d3a7e29e0db42ba01078556e0038443432d2e`  
		Last Modified: Thu, 18 Nov 2021 11:10:46 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3445573f7f6254b2ba9e0154b0ec694a5371151d5a479bd86df27f0db054fa`  
		Last Modified: Thu, 18 Nov 2021 11:10:50 GMT  
		Size: 36.5 MB (36516832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:6.1.0`

```console
$ docker pull lightstreamer@sha256:d817c4f9d46352fc9f311e929c8a50744c999e8ee9b3588b61ff48d037c8e7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:6.1.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:1ad2a23fc88f4a10c96bb7b657ee5653b57f2758cc038aa6ceeb7eb281ee7cab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273462933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55a0c8dd58923ae8ddc551cd8cf574bdc83518ad0d577adf541c99d2e453808`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:07:21 GMT
MAINTAINER Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:07:32 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:07:32 GMT
ENV LIGHSTREAMER_EDITION=Allegro-Presto-Vivace
# Thu, 18 Nov 2021 11:07:48 GMT
ENV LIGHSTREAMER_VERSION=6_1_0_20170123
# Thu, 18 Nov 2021 11:07:49 GMT
ENV LIGHSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_Allegro-Presto-Vivace_6_1_0_20170123.tar.gz
# Thu, 18 Nov 2021 11:07:49 GMT
WORKDIR /lightstreamer
# Thu, 18 Nov 2021 11:07:59 GMT
RUN set -x         && curl -fSL -o Lightstreamer.tar.gz ${LIGHSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e '123,$s/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<appender-ref ref="LSDailyRolling" \/>/ d' conf/lightstreamer_log_conf.xml
# Thu, 18 Nov 2021 11:07:59 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:00 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:00 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328f508a7a13aec2494ba929c34edde250cc8ed239e0764f0d8df13fd1521c5`  
		Last Modified: Thu, 18 Nov 2021 11:10:32 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d141a8b552c80abb6862a627de1d3a7e29e0db42ba01078556e0038443432d2e`  
		Last Modified: Thu, 18 Nov 2021 11:10:46 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3445573f7f6254b2ba9e0154b0ec694a5371151d5a479bd86df27f0db054fa`  
		Last Modified: Thu, 18 Nov 2021 11:10:50 GMT  
		Size: 36.5 MB (36516832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk11`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk8`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7-jdk8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk11`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk8`

```console
$ docker pull lightstreamer@sha256:91e69dcb7aae8e989c37b83802e9c7045085ce1cacf252e489e0f51475973ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:0ba1659c9d5e0b028fa20cbcfb20ad9d5381933e2d74268d7efcdca05804cd45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.4 MB (270401991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9553c17b5841632611bd6efd6767105d4a906509a3aec604ca1e3cedd8109dc2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:22 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:22 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:22 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:22 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:23 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee5269ea29f5c27a4a0aa0aa5efc186291e4858c343f7fefdaed6d30aa0196`  
		Last Modified: Thu, 18 Nov 2021 11:11:05 GMT  
		Size: 33.5 MB (33456026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:91e69dcb7aae8e989c37b83802e9c7045085ce1cacf252e489e0f51475973ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:0ba1659c9d5e0b028fa20cbcfb20ad9d5381933e2d74268d7efcdca05804cd45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.4 MB (270401991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9553c17b5841632611bd6efd6767105d4a906509a3aec604ca1e3cedd8109dc2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:22 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:22 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:22 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:22 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:23 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee5269ea29f5c27a4a0aa0aa5efc186291e4858c343f7fefdaed6d30aa0196`  
		Last Modified: Thu, 18 Nov 2021 11:11:05 GMT  
		Size: 33.5 MB (33456026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk11`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:835675ac236c61b94517d7b3d534c03ce76cf4d732452ba17c7f6b5acc049d6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.0.3-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:912fa010454204fe98dc583bfa92b532295afff00bd706b2d77596575da0fd65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367521871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da84ace0ec684f98f8c1d88cfb7d6547460a2f3b0142ba38266270106378efd`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:30 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:31 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:40 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:40 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:41 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:41 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:41 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8da8ea4030ba6d261c180d37ff4710d00cf7c8255810fc6bd142ebca219598`  
		Last Modified: Thu, 18 Nov 2021 11:11:23 GMT  
		Size: 33.5 MB (33456058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.0.3-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:52807deb4e8f28017ed502c5a5a4555cb6e87a1d3d5fa830a838c0579ade7d11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363473120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e00ee36872489e354ecdee183667f99b1f6116c9333e08ea0c5e5735c286587`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:26:42 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 06:26:43 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 06:26:54 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:26:54 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:26:55 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:26:56 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:26:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fc5192dca5fb699d6b2ea11af0553d9b37e82136a43b47d1c99e17ecb8c3f`  
		Last Modified: Thu, 18 Nov 2021 06:29:27 GMT  
		Size: 33.5 MB (33455866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk8`

```console
$ docker pull lightstreamer@sha256:91e69dcb7aae8e989c37b83802e9c7045085ce1cacf252e489e0f51475973ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0.3-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:0ba1659c9d5e0b028fa20cbcfb20ad9d5381933e2d74268d7efcdca05804cd45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.4 MB (270401991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9553c17b5841632611bd6efd6767105d4a906509a3aec604ca1e3cedd8109dc2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:22 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:22 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:22 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:22 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:23 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee5269ea29f5c27a4a0aa0aa5efc186291e4858c343f7fefdaed6d30aa0196`  
		Last Modified: Thu, 18 Nov 2021 11:11:05 GMT  
		Size: 33.5 MB (33456026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.0.3-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:91e69dcb7aae8e989c37b83802e9c7045085ce1cacf252e489e0f51475973ffe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.0.3-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:0ba1659c9d5e0b028fa20cbcfb20ad9d5381933e2d74268d7efcdca05804cd45
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.4 MB (270401991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9553c17b5841632611bd6efd6767105d4a906509a3aec604ca1e3cedd8109dc2`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_VERSION=7_0_3_20190107
# Thu, 18 Nov 2021 11:08:12 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_0_3_20190107.tar.gz
# Thu, 18 Nov 2021 11:08:22 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && rm -fr /lightstreamer/DOCS-SDKs         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:22 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:22 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:22 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:23 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee5269ea29f5c27a4a0aa0aa5efc186291e4858c343f7fefdaed6d30aa0196`  
		Last Modified: Thu, 18 Nov 2021 11:11:05 GMT  
		Size: 33.5 MB (33456026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk11`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk8`

```console
$ docker pull lightstreamer@sha256:cbce901c0c35e8de4544b6b30573a3d245ddd2bdd6d4506e2102ea53d093eef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:2f97f13c17af1c3404e3ac0f2cf443905097432588d7192d381975718dbcb960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (287040078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b3b482ec2b59e7acda447c564f6963e60db2925daaf27fecd9b860904b75837`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:08:56 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:56 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:56 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:57 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d708d9baf8d51a1885962ad164a462e0bf1c6415526114e0340c6172162f3c3c`  
		Last Modified: Thu, 18 Nov 2021 11:11:47 GMT  
		Size: 50.1 MB (50094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:cbce901c0c35e8de4544b6b30573a3d245ddd2bdd6d4506e2102ea53d093eef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:2f97f13c17af1c3404e3ac0f2cf443905097432588d7192d381975718dbcb960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (287040078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b3b482ec2b59e7acda447c564f6963e60db2925daaf27fecd9b860904b75837`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:08:56 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:56 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:56 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:57 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d708d9baf8d51a1885962ad164a462e0bf1c6415526114e0340c6172162f3c3c`  
		Last Modified: Thu, 18 Nov 2021 11:11:47 GMT  
		Size: 50.1 MB (50094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.2`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.2` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.2` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.2-jdk11`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.2-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.2-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.2-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:22110c2fae1d2b4d46fa71a3f61b7b2ab03d09d5285c8d933aea7dc8b3a7293b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.1.2-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:ca98925360c29ac1ae21ccaece7a3d6ebd12bc5a3ab4ec00f3cd05aecd5c1f09
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.2 MB (384159816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79e4ec9f13495d92b470c5ca3de703ed96edaa100ee07c23fa34954dfacd0ed`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:30 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:09:00 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:09:10 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:11 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:11 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:11 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:11 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bb3471b6f814e3861ff8ccf0f89bac8412f0ee78e3cd18036f3e6508d314cd`  
		Last Modified: Thu, 18 Nov 2021 11:11:21 GMT  
		Size: 2.4 KB (2414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6170413e1b9e6b3cec5b1fcf41f76abdaf7e3dc1b2082646b05e3ee23d484611`  
		Last Modified: Thu, 18 Nov 2021 11:12:05 GMT  
		Size: 50.1 MB (50094003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.1.2-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:6358d5796971356052134142b95f16fe84f9edc053befc556d34a67d1af27bfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.1 MB (380111159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fd5850c573da876f8ad18cd5c4a9907fcb31d1ddcc36d5e761314e9eafa8ff`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:26:41 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:04 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 06:27:05 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 06:27:17 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:18 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:18 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:19 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:20 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55269549c4fd55981e6bcbe33cf7ce0207964a8841db7f10bb84e22c40109bed`  
		Last Modified: Thu, 18 Nov 2021 06:29:23 GMT  
		Size: 2.4 KB (2379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff73ca3eed0bc89fbb85c9fd604aaf18217b97d1095556d95a47b75192bde49`  
		Last Modified: Thu, 18 Nov 2021 06:29:55 GMT  
		Size: 50.1 MB (50093905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.2-jdk8`

```console
$ docker pull lightstreamer@sha256:cbce901c0c35e8de4544b6b30573a3d245ddd2bdd6d4506e2102ea53d093eef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1.2-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:2f97f13c17af1c3404e3ac0f2cf443905097432588d7192d381975718dbcb960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (287040078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b3b482ec2b59e7acda447c564f6963e60db2925daaf27fecd9b860904b75837`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:08:56 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:56 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:56 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:57 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d708d9baf8d51a1885962ad164a462e0bf1c6415526114e0340c6172162f3c3c`  
		Last Modified: Thu, 18 Nov 2021 11:11:47 GMT  
		Size: 50.1 MB (50094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.1.2-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:cbce901c0c35e8de4544b6b30573a3d245ddd2bdd6d4506e2102ea53d093eef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `lightstreamer:7.1.2-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:2f97f13c17af1c3404e3ac0f2cf443905097432588d7192d381975718dbcb960
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.0 MB (287040078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b3b482ec2b59e7acda447c564f6963e60db2925daaf27fecd9b860904b75837`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:08:12 GMT
RUN gpg --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_VERSION=7_1_2
# Thu, 18 Nov 2021 11:08:46 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=http://www.lightstreamer.com/repo/distros/Lightstreamer_7_1_2.tar.gz
# Thu, 18 Nov 2021 11:08:56 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -- 's/\/usr\/jdk1.8.0/$JAVA_HOME/' bin/unix-like/LS.sh         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:08:56 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:08:56 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:08:57 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:08:57 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849cd1e24f61b68b7de457c7edb31491ed423597cb5e0e423bde5e78e5e885e`  
		Last Modified: Thu, 18 Nov 2021 11:11:03 GMT  
		Size: 2.4 KB (2407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d708d9baf8d51a1885962ad164a462e0bf1c6415526114e0340c6172162f3c3c`  
		Last Modified: Thu, 18 Nov 2021 11:11:47 GMT  
		Size: 50.1 MB (50094113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jd8-openjdk`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jd8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jd8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk11`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2-jdk8`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.0`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.0` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.0` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.0-jdk11`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.0-jdk11` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.0-jdk11` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.0-jdk11-openjdk`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.0-jdk11-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.0-jdk11-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.0-jdk8`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.0-jdk8` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.0-jdk8` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:7.2.0-jdk8-openjdk`

```console
$ docker pull lightstreamer@sha256:8f53f476caab7e0d2209295a56499b3c6e36a4a4480cbf8614ba0766e1d75597
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:7.2.0-jdk8-openjdk` - linux; amd64

```console
$ docker pull lightstreamer@sha256:5f99917f9f9d5114276ac1b39f4502b04e3751efaa528335b38fa784ece88484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.3 MB (288266670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e900b393c40a63c2df995f32804c5e2742a2d93223cba22609542a842890d5`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:32:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 09:32:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:32:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:32:15 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:32:15 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 09:32:28 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 11:08:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:35 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:36 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:46 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:47 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:47 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:47 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:47 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f90d4f439f6d7bb6f3034b9c65cf865c13746acd8051c9683ffdb0e8dee4b`  
		Last Modified: Wed, 17 Nov 2021 09:50:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e3bcd577c3a6527e2aab1e2d1f9ba9bff0d993b00230c80c5ae0f9d34a995`  
		Last Modified: Wed, 17 Nov 2021 09:50:40 GMT  
		Size: 106.0 MB (105998958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b8f1da0627f161175029c887ab5652ab449a90fa31f20c7a4f0bb80a622b9e`  
		Last Modified: Thu, 18 Nov 2021 11:13:04 GMT  
		Size: 2.4 KB (2394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857ac576a09b73ae283ceb0954bc0e6303deee69c13d450f7737705ade698719`  
		Last Modified: Thu, 18 Nov 2021 11:13:09 GMT  
		Size: 51.3 MB (51320718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:7.2.0-jdk8-openjdk` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0036acb93c9aa92904ffa29ceba870bde3714504efdf510d68ed9090f97b9740
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285636461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b68e80ab00e0076b6cd6ae9bf5eb6e7a7e955714399aa1f4c760931b111ead`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:59:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 17 Nov 2021 21:59:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:59:48 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:59:49 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:59:50 GMT
ENV JAVA_VERSION=8u312
# Wed, 17 Nov 2021 22:00:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 18 Nov 2021 06:28:02 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:28:09 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:28:10 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:28:11 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:28:23 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:28:23 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:28:24 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:28:25 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:28:26 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917f12eaeac9d9d8bbe5abeddb0acec53266047383c5674de16c2ae3dcb1f534`  
		Last Modified: Wed, 17 Nov 2021 22:15:28 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b7d14e4cba1dfee94560c0015367443403ee970f708a8faa1b698e1f7d06dd`  
		Last Modified: Wed, 17 Nov 2021 22:15:39 GMT  
		Size: 105.0 MB (105010898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0abcab0958cf418e469f61d903f1c05b5b5999532f4b3f68441b1ae0f422b51`  
		Last Modified: Thu, 18 Nov 2021 06:31:00 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab40c24009b8b79093b2f3b6f72a81396c05d0b191ef99f09eea6cf2fce14d`  
		Last Modified: Thu, 18 Nov 2021 06:31:05 GMT  
		Size: 51.3 MB (51320597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `lightstreamer:latest`

```console
$ docker pull lightstreamer@sha256:0701b764cda784d2a2267c532672001594fabec87a158a356bc0dc6c8e21ee52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `lightstreamer:latest` - linux; amd64

```console
$ docker pull lightstreamer@sha256:3d6136436893db7d9bc6db5502c69b9edb5609db95bc60e119510eac3216c4b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.4 MB (385386508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6148683637c4d1ca1c85dd129f8aaad277d9292708c544aaf942729add1cbe79`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:14:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:28:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 09:28:03 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 09:28:04 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 09:28:04 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:28:04 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 09:28:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 09:28:36 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 11:08:26 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 11:09:19 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 11:09:19 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 11:09:30 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 11:09:30 GMT
USER lightstreamer
# Thu, 18 Nov 2021 11:09:30 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 11:09:31 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 11:09:31 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5576ce26bf1df68da60eeb5162dccde1b69f865d2815aba8b2d29e7181aeb62b`  
		Last Modified: Wed, 17 Nov 2021 03:23:31 GMT  
		Size: 54.6 MB (54566324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26518d6c686a233a54207844e4b7d3b6d61257949d6ad066f69d7a71a6a372aa`  
		Last Modified: Wed, 17 Nov 2021 09:46:01 GMT  
		Size: 5.4 MB (5420096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1f4e0dbfd41d06a54d449884e69cc8d0e912dcc0992a4e38372388e96d98a`  
		Last Modified: Wed, 17 Nov 2021 09:45:59 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d872b5136cc5107372f49c8e70da9ff97147824c50d2b88be26a6ac5accc1a3`  
		Last Modified: Wed, 17 Nov 2021 09:46:20 GMT  
		Size: 203.1 MB (203118803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d021928a056ae8ae7d4f292d474c5a695c0fff76bddad1493970265bc4703c2`  
		Last Modified: Thu, 18 Nov 2021 11:12:28 GMT  
		Size: 2.4 KB (2405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549c8d66ff958f5c6ace49d3961cc722fd9a7137b41a03d293a14f2624005c80`  
		Last Modified: Thu, 18 Nov 2021 11:12:32 GMT  
		Size: 51.3 MB (51320704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `lightstreamer:latest` - linux; arm64 variant v8

```console
$ docker pull lightstreamer@sha256:0bfb9ea76cd077b67dc85011fa430f949de70604af7151a2f262fa7def43a990
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.3 MB (381337799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1da9898623ca0d8fe93c84172b0e767cc83e91a665e0f49fad59d23d587c0ac`
-	Default Command: `[".\/LS.sh","run"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:27:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:56:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 17 Nov 2021 21:56:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 17 Nov 2021 21:56:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Nov 2021 21:56:55 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 21:56:56 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 17 Nov 2021 21:57:20 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 17 Nov 2021 21:57:20 GMT
CMD ["jshell"]
# Thu, 18 Nov 2021 06:26:32 GMT
LABEL maintainer=Lightstreamer Server Development Team <support@lightstreamer.com>
# Thu, 18 Nov 2021 06:27:36 GMT
RUN gpg --batch --keyserver hkp://keyserver.ubuntu.com --recv-keys 9B90BFD14309C7DA5EF58D7D4A8C08966F29B4D2
# Thu, 18 Nov 2021 06:27:37 GMT
ENV LIGHTSTREAMER_VERSION=7_2_0
# Thu, 18 Nov 2021 06:27:38 GMT
ENV LIGHTSTREAMER_URL_DOWNLOAD=https://www.lightstreamer.com/repo/distros/Lightstreamer_7_2_0.tar.gz
# Thu, 18 Nov 2021 06:27:50 GMT
RUN set -ex;         mkdir /lightstreamer && cd /lightstreamer         && curl -fSL -o Lightstreamer.tar.gz ${LIGHTSTREAMER_URL_DOWNLOAD}         && curl -fSL -o Lightstreamer.tar.gz.asc ${LIGHTSTREAMER_URL_DOWNLOAD}.asc         && gpg --batch --verify Lightstreamer.tar.gz.asc Lightstreamer.tar.gz         && tar -xvf Lightstreamer.tar.gz --strip-components=1         && sed -i -e 's/<appender-ref ref="LSDailyRolling" \/>/<appender-ref ref="LSConsole" \/>/'                   -e '/<logger name="LightstreamerLogger.init/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerLogger.license/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   -e '/<logger name="LightstreamerProxyAdapters/,+2s/<appender-ref ref="LSConsole" \/>/<!-- <appender-ref ref="LSConsole" \/> -->/'                   conf/lightstreamer_log_conf.xml         && groupadd -r -g 10000 lightstreamer         && useradd --no-log-init -r -g lightstreamer -u 10000 lightstreamer         && chown -R lightstreamer:lightstreamer ../lightstreamer         && rm Lightstreamer.tar.gz Lightstreamer.tar.gz.asc
# Thu, 18 Nov 2021 06:27:50 GMT
USER lightstreamer
# Thu, 18 Nov 2021 06:27:51 GMT
EXPOSE 8080
# Thu, 18 Nov 2021 06:27:52 GMT
WORKDIR /lightstreamer/bin/unix-like
# Thu, 18 Nov 2021 06:27:53 GMT
CMD ["./LS.sh" "run"]
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7a1cfcc2070fbe1e702751d85f7074b93d142f6beb03ef66e9ba1c58bcc3e3`  
		Last Modified: Wed, 17 Nov 2021 13:36:49 GMT  
		Size: 54.7 MB (54669696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ad2e26f24303b213a44df57da171fefb54e8669fc653ed178587d765c68cf5`  
		Last Modified: Wed, 17 Nov 2021 22:12:54 GMT  
		Size: 5.4 MB (5420139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4190b07ffffe33edc1362c33a1637f45de6076e8ae7514f6927252facd8240`  
		Last Modified: Wed, 17 Nov 2021 22:12:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfecab53ca4466c76e8146d133e5cdaffe910f9e4009144e0e56b27ff63b6d`  
		Last Modified: Wed, 17 Nov 2021 22:13:11 GMT  
		Size: 200.7 MB (200712287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7714a2d28da43ece69cfbf0598b8e747979d0eac1611358c5765ed498e518c`  
		Last Modified: Thu, 18 Nov 2021 06:30:19 GMT  
		Size: 2.4 KB (2377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665d004633b3d77eb7f693927b4ff452424c0ed752f1d54009e65f9509159d9`  
		Last Modified: Thu, 18 Nov 2021 06:30:27 GMT  
		Size: 51.3 MB (51320547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
