<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `flink`

-	[`flink:1.12`](#flink112)
-	[`flink:1.12-java11`](#flink112-java11)
-	[`flink:1.12-java8`](#flink112-java8)
-	[`flink:1.12-scala_2.11`](#flink112-scala_211)
-	[`flink:1.12-scala_2.11-java11`](#flink112-scala_211-java11)
-	[`flink:1.12-scala_2.11-java8`](#flink112-scala_211-java8)
-	[`flink:1.12-scala_2.12`](#flink112-scala_212)
-	[`flink:1.12-scala_2.12-java11`](#flink112-scala_212-java11)
-	[`flink:1.12-scala_2.12-java8`](#flink112-scala_212-java8)
-	[`flink:1.12.4`](#flink1124)
-	[`flink:1.12.4-java11`](#flink1124-java11)
-	[`flink:1.12.4-java8`](#flink1124-java8)
-	[`flink:1.12.4-scala_2.11`](#flink1124-scala_211)
-	[`flink:1.12.4-scala_2.11-java11`](#flink1124-scala_211-java11)
-	[`flink:1.12.4-scala_2.11-java8`](#flink1124-scala_211-java8)
-	[`flink:1.12.4-scala_2.12`](#flink1124-scala_212)
-	[`flink:1.12.4-scala_2.12-java11`](#flink1124-scala_212-java11)
-	[`flink:1.12.4-scala_2.12-java8`](#flink1124-scala_212-java8)
-	[`flink:1.13`](#flink113)
-	[`flink:1.13-java11`](#flink113-java11)
-	[`flink:1.13-java8`](#flink113-java8)
-	[`flink:1.13-scala_2.11`](#flink113-scala_211)
-	[`flink:1.13-scala_2.11-java11`](#flink113-scala_211-java11)
-	[`flink:1.13-scala_2.11-java8`](#flink113-scala_211-java8)
-	[`flink:1.13-scala_2.12`](#flink113-scala_212)
-	[`flink:1.13-scala_2.12-java11`](#flink113-scala_212-java11)
-	[`flink:1.13-scala_2.12-java8`](#flink113-scala_212-java8)
-	[`flink:1.13.1`](#flink1131)
-	[`flink:1.13.1-java11`](#flink1131-java11)
-	[`flink:1.13.1-java8`](#flink1131-java8)
-	[`flink:1.13.1-scala_2.11`](#flink1131-scala_211)
-	[`flink:1.13.1-scala_2.11-java11`](#flink1131-scala_211-java11)
-	[`flink:1.13.1-scala_2.11-java8`](#flink1131-scala_211-java8)
-	[`flink:1.13.1-scala_2.12`](#flink1131-scala_212)
-	[`flink:1.13.1-scala_2.12-java11`](#flink1131-scala_212-java11)
-	[`flink:1.13.1-scala_2.12-java8`](#flink1131-scala_212-java8)
-	[`flink:java11`](#flinkjava11)
-	[`flink:java8`](#flinkjava8)
-	[`flink:latest`](#flinklatest)
-	[`flink:scala_2.11`](#flinkscala_211)
-	[`flink:scala_2.11-java11`](#flinkscala_211-java11)
-	[`flink:scala_2.11-java8`](#flinkscala_211-java8)
-	[`flink:scala_2.12`](#flinkscala_212)
-	[`flink:scala_2.12-java11`](#flinkscala_212-java11)
-	[`flink:scala_2.12-java8`](#flinkscala_212-java8)

## `flink:1.12`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-java11`

```console
$ docker pull flink@sha256:349eb56ce67aecc372225bac81e6b7a1200e0e004b611b49afb1ef4c0577bf46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:f60e982374cfcec9fe303590e6d3a29e0b5381b00f07d98e3e5a42dff2672ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449070472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ef346210a1525e44b0608386e96f7b150e78c7b2d77e1ba0b28c33512bcd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:36:35 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:36:35 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:36:36 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:52 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:53 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:53 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:54 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64f08ad6f4a6a3b02e4fe2afd8b3b3415a04f48461fdcd3c06dececff7346f`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7750704f77abab4aa881cb198b0ae2f6ca80a42951c2a1ea68690f921ed13c20`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5baf83c6f8f0929a560cf02241bc809eeef30aefa3670dcfad8b59753982f8`  
		Last Modified: Tue, 25 May 2021 18:43:05 GMT  
		Size: 326.0 MB (326011453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff2af535e71ccee02159f9f7a80f978932f9c26c3713f96011cb2c70c6358cb`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-java8`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.11`

```console
$ docker pull flink@sha256:796b571b5090316d0b67509a19fdd2b7b684270f9cb86ee6bd2b2ea840a483ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:1348408c68731e9d9dec9c87e291bfb633ecb91d760908581eb6a481298a31c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.0 MB (452982363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a842ceff555e378a54129f3bea192e569a990a27638a941de62765a9a367f8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:00 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:01 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:01 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:37:32 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:37:33 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:37:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:37:34 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:37:34 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f924c4e54f07fc9a2f1f463cd24832a99a5feeef107d2c91ca4a591f929d1`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8061d7d9c59ea1f0f01aef1e93912ddc4aa72ef75e0871617e3eda93e32a2`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076ce08406506ab8fc15fdb5f0b4d3a48814c0388feb2085a279dec66abeede3`  
		Last Modified: Tue, 25 May 2021 18:43:43 GMT  
		Size: 335.4 MB (335405649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e689b3768ca0bc99be9461272a7b06b2f0b8df09a3e5f2a3b7631d022b782`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.11-java11`

```console
$ docker pull flink@sha256:5bc0abcd1775aa9d36ecc80b423ef86e9e14e2ad768b34dd64895650c095df23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:46f60ceb74c14fa54fac5128bbc105e8726beac63bed649c7b353390ad1db55a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.5 MB (458464612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b7c3006868fd64750cc48efeda847d50386f2187f0cbd6ae8d5bd4039c9ed7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:42 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:42 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:43 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:44 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:44 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:38:12 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:38:13 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:38:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:38:13 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:38:13 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150dcb5caf9e3ae1e760548555686950bd3609048e4e5d895dafca04181de388`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff2cc68f11477f2a7dfaad11d6b2031176c46433fade13843c88081d0be85ec`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41887f4903029df02eda5e802d13b99b2ef298c085790970b661da271afa42bf`  
		Last Modified: Tue, 25 May 2021 18:44:18 GMT  
		Size: 335.4 MB (335405595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35f180a44ab48d095a4515a1c3be024af614d55462dc8320605e2e7b6cf3f91`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.11-java8`

```console
$ docker pull flink@sha256:796b571b5090316d0b67509a19fdd2b7b684270f9cb86ee6bd2b2ea840a483ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:1348408c68731e9d9dec9c87e291bfb633ecb91d760908581eb6a481298a31c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.0 MB (452982363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a842ceff555e378a54129f3bea192e569a990a27638a941de62765a9a367f8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:00 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:01 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:01 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:37:32 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:37:33 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:37:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:37:34 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:37:34 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f924c4e54f07fc9a2f1f463cd24832a99a5feeef107d2c91ca4a591f929d1`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8061d7d9c59ea1f0f01aef1e93912ddc4aa72ef75e0871617e3eda93e32a2`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076ce08406506ab8fc15fdb5f0b4d3a48814c0388feb2085a279dec66abeede3`  
		Last Modified: Tue, 25 May 2021 18:43:43 GMT  
		Size: 335.4 MB (335405649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e689b3768ca0bc99be9461272a7b06b2f0b8df09a3e5f2a3b7631d022b782`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.12`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.12-java11`

```console
$ docker pull flink@sha256:349eb56ce67aecc372225bac81e6b7a1200e0e004b611b49afb1ef4c0577bf46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:f60e982374cfcec9fe303590e6d3a29e0b5381b00f07d98e3e5a42dff2672ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449070472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ef346210a1525e44b0608386e96f7b150e78c7b2d77e1ba0b28c33512bcd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:36:35 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:36:35 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:36:36 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:52 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:53 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:53 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:54 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64f08ad6f4a6a3b02e4fe2afd8b3b3415a04f48461fdcd3c06dececff7346f`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7750704f77abab4aa881cb198b0ae2f6ca80a42951c2a1ea68690f921ed13c20`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5baf83c6f8f0929a560cf02241bc809eeef30aefa3670dcfad8b59753982f8`  
		Last Modified: Tue, 25 May 2021 18:43:05 GMT  
		Size: 326.0 MB (326011453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff2af535e71ccee02159f9f7a80f978932f9c26c3713f96011cb2c70c6358cb`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12-scala_2.12-java8`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-java11`

```console
$ docker pull flink@sha256:349eb56ce67aecc372225bac81e6b7a1200e0e004b611b49afb1ef4c0577bf46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-java11` - linux; amd64

```console
$ docker pull flink@sha256:f60e982374cfcec9fe303590e6d3a29e0b5381b00f07d98e3e5a42dff2672ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449070472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ef346210a1525e44b0608386e96f7b150e78c7b2d77e1ba0b28c33512bcd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:36:35 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:36:35 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:36:36 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:52 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:53 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:53 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:54 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64f08ad6f4a6a3b02e4fe2afd8b3b3415a04f48461fdcd3c06dececff7346f`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7750704f77abab4aa881cb198b0ae2f6ca80a42951c2a1ea68690f921ed13c20`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5baf83c6f8f0929a560cf02241bc809eeef30aefa3670dcfad8b59753982f8`  
		Last Modified: Tue, 25 May 2021 18:43:05 GMT  
		Size: 326.0 MB (326011453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff2af535e71ccee02159f9f7a80f978932f9c26c3713f96011cb2c70c6358cb`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-java8`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-java8` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.11`

```console
$ docker pull flink@sha256:796b571b5090316d0b67509a19fdd2b7b684270f9cb86ee6bd2b2ea840a483ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:1348408c68731e9d9dec9c87e291bfb633ecb91d760908581eb6a481298a31c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.0 MB (452982363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a842ceff555e378a54129f3bea192e569a990a27638a941de62765a9a367f8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:00 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:01 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:01 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:37:32 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:37:33 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:37:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:37:34 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:37:34 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f924c4e54f07fc9a2f1f463cd24832a99a5feeef107d2c91ca4a591f929d1`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8061d7d9c59ea1f0f01aef1e93912ddc4aa72ef75e0871617e3eda93e32a2`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076ce08406506ab8fc15fdb5f0b4d3a48814c0388feb2085a279dec66abeede3`  
		Last Modified: Tue, 25 May 2021 18:43:43 GMT  
		Size: 335.4 MB (335405649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e689b3768ca0bc99be9461272a7b06b2f0b8df09a3e5f2a3b7631d022b782`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.11-java11`

```console
$ docker pull flink@sha256:5bc0abcd1775aa9d36ecc80b423ef86e9e14e2ad768b34dd64895650c095df23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:46f60ceb74c14fa54fac5128bbc105e8726beac63bed649c7b353390ad1db55a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.5 MB (458464612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b7c3006868fd64750cc48efeda847d50386f2187f0cbd6ae8d5bd4039c9ed7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:42 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:42 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:43 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:44 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:44 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:38:12 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:38:13 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:38:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:38:13 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:38:13 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150dcb5caf9e3ae1e760548555686950bd3609048e4e5d895dafca04181de388`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff2cc68f11477f2a7dfaad11d6b2031176c46433fade13843c88081d0be85ec`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41887f4903029df02eda5e802d13b99b2ef298c085790970b661da271afa42bf`  
		Last Modified: Tue, 25 May 2021 18:44:18 GMT  
		Size: 335.4 MB (335405595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35f180a44ab48d095a4515a1c3be024af614d55462dc8320605e2e7b6cf3f91`  
		Last Modified: Tue, 25 May 2021 18:44:01 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.11-java8`

```console
$ docker pull flink@sha256:796b571b5090316d0b67509a19fdd2b7b684270f9cb86ee6bd2b2ea840a483ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:1348408c68731e9d9dec9c87e291bfb633ecb91d760908581eb6a481298a31c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **453.0 MB (452982363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a842ceff555e378a54129f3bea192e569a990a27638a941de62765a9a367f8c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.11.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:37:00 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:37:00 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:37:01 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:37:01 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:37:32 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:37:33 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:37:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:37:34 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:37:34 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f924c4e54f07fc9a2f1f463cd24832a99a5feeef107d2c91ca4a591f929d1`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e8061d7d9c59ea1f0f01aef1e93912ddc4aa72ef75e0871617e3eda93e32a2`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076ce08406506ab8fc15fdb5f0b4d3a48814c0388feb2085a279dec66abeede3`  
		Last Modified: Tue, 25 May 2021 18:43:43 GMT  
		Size: 335.4 MB (335405649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e689b3768ca0bc99be9461272a7b06b2f0b8df09a3e5f2a3b7631d022b782`  
		Last Modified: Tue, 25 May 2021 18:43:27 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.12`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.12-java11`

```console
$ docker pull flink@sha256:349eb56ce67aecc372225bac81e6b7a1200e0e004b611b49afb1ef4c0577bf46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:f60e982374cfcec9fe303590e6d3a29e0b5381b00f07d98e3e5a42dff2672ed8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449070472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ef346210a1525e44b0608386e96f7b150e78c7b2d77e1ba0b28c33512bcd1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:36:34 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:36:35 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:36:35 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:36:36 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:52 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:53 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:53 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:54 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a64f08ad6f4a6a3b02e4fe2afd8b3b3415a04f48461fdcd3c06dececff7346f`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7750704f77abab4aa881cb198b0ae2f6ca80a42951c2a1ea68690f921ed13c20`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5baf83c6f8f0929a560cf02241bc809eeef30aefa3670dcfad8b59753982f8`  
		Last Modified: Tue, 25 May 2021 18:43:05 GMT  
		Size: 326.0 MB (326011453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff2af535e71ccee02159f9f7a80f978932f9c26c3713f96011cb2c70c6358cb`  
		Last Modified: Tue, 25 May 2021 18:42:49 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.12.4-scala_2.12-java8`

```console
$ docker pull flink@sha256:8bed67835d2e6b3bd62831476c3ddb48c9702d2c0615c2c67b2472a55cbb3a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.12.4-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:b61a8b212299c74e3526b484e690d01131bd490d9fe067da25fa15d1a32e9232
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **443.6 MB (443588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5081c73070e5ea85d75cbcda43f4376f895e8d7750f2e4b9550bb60c9856ea1e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.12.4/flink-1.12.4-bin-scala_2.12.tgz.asc GPG_KEY=A53C7D531C6889386EB6D94E476DAA5D1FF08189 CHECK_GPG=true
# Tue, 25 May 2021 18:25:50 GMT
ENV FLINK_HOME=/opt/flink
# Tue, 25 May 2021 18:25:50 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 May 2021 18:25:51 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Tue, 25 May 2021 18:25:52 GMT
WORKDIR /opt/flink
# Tue, 25 May 2021 18:36:20 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Tue, 25 May 2021 18:36:21 GMT
COPY file:169fc968df81e9941ad72fb5a70e8f5ef9e97e9bc4e58e8f596f13fbaaf8ab4f in / 
# Tue, 25 May 2021 18:36:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 25 May 2021 18:36:21 GMT
EXPOSE 6123 8081
# Tue, 25 May 2021 18:36:22 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305f898c5855aba3c622c800e60ef71988005fb7eb24c5aea7d503d317e0cc5d`  
		Last Modified: Tue, 25 May 2021 18:41:59 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735132022efcfc238bf96e505587ad8f878bc773ae51c1e1c259617c4b696cd2`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc511b793fb364273792800f1e3fce6f203cd37c10a917528908ad576b506d`  
		Last Modified: Tue, 25 May 2021 18:42:16 GMT  
		Size: 326.0 MB (326011458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b579ad985156a47dfc17a74382f2fcf33dab3995c450337920613651baa3dc`  
		Last Modified: Tue, 25 May 2021 18:41:58 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.11`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.11-java11`

```console
$ docker pull flink@sha256:ceb1e965e2bf7af75e4ae12ad4f17fb1212e80624517750b58d6cd9b832c2d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:568488b066cbe80feac426377b1fe65c7ccbd872fadef9fabe2015e7746b9bcd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437713684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09ad788316e8465af8c546bb540003225df73f4e8817481d486908015b7747a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:13:23 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:13:24 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:13:24 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:57 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:58 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:58 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b60d3ee18cae592621cfd77739e2129ad382d364516c093400ef68f83da8bf`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f50b613b9a28d965f04c50863d5193e86e5a29d82ab5afc0e3f3fb5fe11fc2`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e337b06d13d747caa992f2b96c1479d5ae0b0fd08e2a29c0987381baa0e682`  
		Last Modified: Wed, 02 Jun 2021 03:18:41 GMT  
		Size: 314.7 MB (314654888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0486f37de8a498fa0d81f575c828ec78fc6f6f13339db750e96a96172e8fff`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.11-java8`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.12`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.12-java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13-scala_2.12-java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.11`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.11-java11`

```console
$ docker pull flink@sha256:ceb1e965e2bf7af75e4ae12ad4f17fb1212e80624517750b58d6cd9b832c2d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:568488b066cbe80feac426377b1fe65c7ccbd872fadef9fabe2015e7746b9bcd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437713684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09ad788316e8465af8c546bb540003225df73f4e8817481d486908015b7747a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:13:23 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:13:24 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:13:24 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:57 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:58 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:58 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b60d3ee18cae592621cfd77739e2129ad382d364516c093400ef68f83da8bf`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f50b613b9a28d965f04c50863d5193e86e5a29d82ab5afc0e3f3fb5fe11fc2`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e337b06d13d747caa992f2b96c1479d5ae0b0fd08e2a29c0987381baa0e682`  
		Last Modified: Wed, 02 Jun 2021 03:18:41 GMT  
		Size: 314.7 MB (314654888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0486f37de8a498fa0d81f575c828ec78fc6f6f13339db750e96a96172e8fff`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.11-java8`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.12`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.12-java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:1.13.1-scala_2.12-java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:1.13.1-scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:latest`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:latest` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.11`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.11` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.11-java11`

```console
$ docker pull flink@sha256:ceb1e965e2bf7af75e4ae12ad4f17fb1212e80624517750b58d6cd9b832c2d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.11-java11` - linux; amd64

```console
$ docker pull flink@sha256:568488b066cbe80feac426377b1fe65c7ccbd872fadef9fabe2015e7746b9bcd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.7 MB (437713684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09ad788316e8465af8c546bb540003225df73f4e8817481d486908015b7747a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:13:22 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:13:23 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:13:24 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:13:24 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:56 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:57 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:58 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:58 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b60d3ee18cae592621cfd77739e2129ad382d364516c093400ef68f83da8bf`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f50b613b9a28d965f04c50863d5193e86e5a29d82ab5afc0e3f3fb5fe11fc2`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e337b06d13d747caa992f2b96c1479d5ae0b0fd08e2a29c0987381baa0e682`  
		Last Modified: Wed, 02 Jun 2021 03:18:41 GMT  
		Size: 314.7 MB (314654888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0486f37de8a498fa0d81f575c828ec78fc6f6f13339db750e96a96172e8fff`  
		Last Modified: Wed, 02 Jun 2021 03:18:17 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.11-java8`

```console
$ docker pull flink@sha256:42acf339ed56755c31b2b66800f85a2651a227e6a4382799c3c2bf6a18e4e881
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.11-java8` - linux; amd64

```console
$ docker pull flink@sha256:12045f988374123afef33e1f7b51a7a7b4e6273ef06e9008d39b9afeeac4228e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.2 MB (432231358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5cbc176e469b2f877c66eecbdf4b56ee34c7c28bc9c535158e3f68b5320dc1d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:02:53 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.11.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:02:54 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:02:54 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:02:56 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:02:56 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:13:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:13:05 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:13:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:13:05 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:13:05 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9da05b62bad7e6fb79d5cc0948fc83164cd27e2bddde5f0a80d16bc92f874e`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 4.6 KB (4607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561cc0ed0658aeffe246e394abec2546e6ad4d24472ab90eb9cea4fcc222e994`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae889fa70273285ea32a69b2919a0f18982b821cc0e2f93f0e2dd6184ace5a4`  
		Last Modified: Wed, 02 Jun 2021 03:17:50 GMT  
		Size: 314.7 MB (314654863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bdfea2076fe28702fbb7c73080bd0fb28810e4ba4479d10fdad341352c33e7`  
		Last Modified: Wed, 02 Jun 2021 03:17:26 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.12`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.12` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.12-java11`

```console
$ docker pull flink@sha256:c7b976b79045ee8372f1e4d92db283ea23562a7b8a3962942ca323d3f233fac1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.12-java11` - linux; amd64

```console
$ docker pull flink@sha256:6648dd2c8b5a3f524f6ac8f12e29dafd9fb8270bf6e8d048f98a0f27dbb947d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428386083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c032765533fbec147dcb31696b56aa4fdbd8e517bff5ed2bf187b6ff6ec698`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:51:19 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 12 May 2021 06:51:21 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:51:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:51:21 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:51:22 GMT
ENV JAVA_VERSION=11.0.11+9
# Wed, 12 May 2021 06:51:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_linux_11.0.11_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_aarch64_linux_11.0.11_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 25 May 2021 18:23:22 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:23:22 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:23:24 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 03:00:12 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 03:00:12 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 03:00:14 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 03:00:14 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:02:45 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:02:46 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:02:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:02:47 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:02:47 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54652506fa027da77fb33410f69e04defd83d788aeace7fe493fefb1ae0bd191`  
		Last Modified: Wed, 12 May 2021 07:03:50 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032db4689f58114bbe3b69e68cdc395f85606302f874e55ed3159800f370b422`  
		Last Modified: Wed, 12 May 2021 07:04:01 GMT  
		Size: 46.8 MB (46805370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d5a96bf6e6764e31a95dea681b70576b6c3b64fc708975c425aea3f8cd962`  
		Last Modified: Tue, 25 May 2021 18:39:59 GMT  
		Size: 1.6 MB (1551515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f227b25268462f4ac80f530646a9539480c1348535c7d06863198cfb3d6176`  
		Last Modified: Tue, 25 May 2021 18:39:57 GMT  
		Size: 900.5 KB (900540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43014fab0d436e7e8c18886c62f7fd1f4bf212a1e8c286f2bffc1ffebd0bcb22`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 4.6 KB (4605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5d95d79f7d2cba74177ba9198066a9d49772eeb4d6d36461b6c947295649fc`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205ee713c75cef01555a2d40bb4531b72f039c1cf433b79be0f3cb565dade663`  
		Last Modified: Wed, 02 Jun 2021 03:17:00 GMT  
		Size: 305.3 MB (305327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ee53ffbe9dc7a813715dabca576ca89ea0a6ab7b9988994012834a08930911`  
		Last Modified: Wed, 02 Jun 2021 03:16:36 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `flink:scala_2.12-java8`

```console
$ docker pull flink@sha256:9efd47d965e61165b808353ea4656b5d19b5879fb7636cc9901833626c8866a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `flink:scala_2.12-java8` - linux; amd64

```console
$ docker pull flink@sha256:10d229c31ccadfa1a35cf26243d2f14c6d289c8cef8fd2e211958a40c2669668
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.9 MB (422903781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c04db012c1c58646060de94987f7f8842e4493a77cc73d9cc4cc89dbe27d6e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 12 May 2021 01:21:03 GMT
ADD file:1a1eae7a82c66d673971436ce2605e97d107e2934b7cdec876c64923ae6f4f85 in / 
# Wed, 12 May 2021 01:21:03 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:55:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:55:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 06:51:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:52:45 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 12 May 2021 06:52:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 12 May 2021 06:52:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:52:46 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:52:47 GMT
ENV JAVA_VERSION=8u292
# Wed, 12 May 2021 06:52:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_linux_8u292b10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_aarch64_linux_8u292b10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 25 May 2021 18:22:45 GMT
RUN set -ex;   apt-get update;   apt-get -y install libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Tue, 25 May 2021 18:22:45 GMT
ENV GOSU_VERSION=1.11
# Tue, 25 May 2021 18:22:47 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.13.1/flink-1.13.1-bin-scala_2.12.tgz.asc GPG_KEY=31D2DD10BFC15A2D CHECK_GPG=true
# Wed, 02 Jun 2021 02:59:36 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 02 Jun 2021 02:59:36 GMT
ENV PATH=/opt/flink/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Jun 2021 02:59:37 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 02 Jun 2021 02:59:37 GMT
WORKDIR /opt/flink
# Wed, 02 Jun 2021 03:00:03 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;
# Wed, 02 Jun 2021 03:00:04 GMT
COPY file:5cd5e39f1e46b85ff32fa26e988fe4d93983dcbef27712cf760efc65655f7310 in / 
# Wed, 02 Jun 2021 03:00:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Jun 2021 03:00:04 GMT
EXPOSE 6123 8081
# Wed, 02 Jun 2021 03:00:04 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:d960726af2bec62a87ceb07182f7b94c47be03909077e23d8226658f80b47f87`  
		Last Modified: Wed, 12 May 2021 01:26:49 GMT  
		Size: 50.4 MB (50433242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d62473a22dec9ffef056b2017968a9dc484c8f836fb6d79f46980b309e9138`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 7.8 MB (7832938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8962bc0fad55b13afedfeb6ad5cb06fd065461cf3e1ae4e7aeae5eeb17b179df`  
		Last Modified: Wed, 12 May 2021 02:04:42 GMT  
		Size: 10.0 MB (9997157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961f7da1b9e58d2ed3e166d9edac7abb64d17576bb3f509730f052d6b53cf405`  
		Last Modified: Wed, 12 May 2021 07:03:52 GMT  
		Size: 5.5 MB (5531125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba190cfbc66aa38796618592de325cde5937c69d06132ec92489eefae346474`  
		Last Modified: Wed, 12 May 2021 07:06:07 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595e52ef2a1b7942d5075b4678ebba3f49e8216931456bd383fb71c70f115bb1`  
		Last Modified: Wed, 12 May 2021 07:06:13 GMT  
		Size: 41.3 MB (41323156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85477d4a5383d823760c9a129d3ac4a34b7a142af0376f39521d9d7a4cd8a7d`  
		Last Modified: Tue, 25 May 2021 18:39:01 GMT  
		Size: 1.6 MB (1551428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa91174d9bfac2858c172ee00b28464d94bea75d1ac4b297b7efe08ed460f00`  
		Last Modified: Tue, 25 May 2021 18:38:58 GMT  
		Size: 900.5 KB (900537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2a662d3b958310ead39e73684156b4467c349b8d2f12ba4b27fac54db5a5d9`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 4.6 KB (4604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adec0e30bd9871d8e0fe0b6d39769408672001141c3f0ab618f18f73063258a`  
		Last Modified: Wed, 02 Jun 2021 03:15:22 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c768cb3e1942b1d037791bfd56bec011e931f946ea4a4089d7a736220496c4`  
		Last Modified: Wed, 02 Jun 2021 03:15:44 GMT  
		Size: 305.3 MB (305327289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472f0edbb212b14823402b07aecea02128de6d1c2fa77e674c857170c02beed`  
		Last Modified: Wed, 02 Jun 2021 03:15:21 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
