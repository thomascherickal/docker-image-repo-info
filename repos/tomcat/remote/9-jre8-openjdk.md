## `tomcat:9-jre8-openjdk`

```console
$ docker pull tomcat@sha256:5e7323cf74b1e9fa7a8367423f7f3ab311434793b3010973c5f18942e2453963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jre8-openjdk` - linux; amd64

```console
$ docker pull tomcat@sha256:e8b0aee87fbb822eaa67bfa93d8e7601e6b3fc2a087f04e2248e1f03373dc115
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130581290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8c4b4287dc976e7ffb14e57a37644d10856769a118002c9399763f8effb26a7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 16:34:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:36:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 12 Oct 2021 16:36:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Oct 2021 16:36:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:36:58 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:47:52 GMT
ENV JAVA_VERSION=8u312
# Thu, 21 Oct 2021 23:47:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 22 Oct 2021 00:27:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 Oct 2021 00:27:11 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Oct 2021 00:27:11 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 Oct 2021 00:27:12 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 Oct 2021 00:27:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 Oct 2021 00:27:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 Oct 2021 00:37:43 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 22 Oct 2021 00:37:43 GMT
ENV TOMCAT_MAJOR=9
# Fri, 22 Oct 2021 00:37:43 GMT
ENV TOMCAT_VERSION=9.0.54
# Fri, 22 Oct 2021 00:37:44 GMT
ENV TOMCAT_SHA512=83430f24d42186ce2ff51eeef2f7a5517048f37d9050c45cac1e3dba8926d61a1f7f5aba122a34a11ac1dbdd3c1f6d98671841047df139394d43751263de57c3
# Fri, 22 Oct 2021 00:37:44 GMT
COPY dir:4ae79e1c2556ec4c3f380bb476a0e7e62186304766ba4ebe82008be7aac1cd2c in /usr/local/tomcat 
# Fri, 22 Oct 2021 00:37:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 00:37:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 Oct 2021 00:37:49 GMT
EXPOSE 8080
# Fri, 22 Oct 2021 00:37:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab18cfab55f9b2e1184b3f5b90de6574c96bdf1c4c782f4e1879437c38541af9`  
		Last Modified: Tue, 12 Oct 2021 16:53:01 GMT  
		Size: 5.7 MB (5653928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793716e93ecb3dc756176dea4353c0fd34b83be7fe04582df89283781c0e2bdf`  
		Last Modified: Tue, 12 Oct 2021 16:56:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9b14f7678b3f0af9568b4869f0100eb02cc4d107d2436284db725c0aabda65`  
		Last Modified: Fri, 22 Oct 2021 00:05:00 GMT  
		Size: 41.4 MB (41372080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2d594b57d6413d65c1791a79189febcd379064f219e565e68f60d82b68bbf`  
		Last Modified: Fri, 22 Oct 2021 01:13:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c253e48bc853bbcaaed9dbea4c6635b0493f7317835cedaac3eea6bcd7034ed`  
		Last Modified: Fri, 22 Oct 2021 01:20:34 GMT  
		Size: 12.2 MB (12152454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367036ef11f2f17ee8cd61e0a5d98f9ffc440a8aaeb1169d130068d50bd4e5bd`  
		Last Modified: Fri, 22 Oct 2021 01:20:33 GMT  
		Size: 459.6 KB (459588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8c81d4f4615180edcda2dd6d3b5109d645a50e13913aa80b780a777d063bdf`  
		Last Modified: Fri, 22 Oct 2021 01:20:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-openjdk` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:6d9200f34a6d4cda7091ff2707528f3f4816d9438a21274c7109414f0930b793
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128045289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112cf3787c05cf9f3c71f4a73843bb7903ed27a729bf8719259cddd5e7afd366`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:04 GMT
ADD file:1529ae12e334fd992892d3fb97c103297cff7e0115b0475bec4c093939a2bff7 in / 
# Tue, 12 Oct 2021 01:41:04 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:58:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 04:11:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 04:14:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sat, 16 Oct 2021 04:14:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Sat, 16 Oct 2021 04:14:03 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 04:14:04 GMT
ENV LANG=C.UTF-8
# Sat, 16 Oct 2021 04:14:05 GMT
ENV JAVA_VERSION=8u302
# Sat, 16 Oct 2021 04:14:11 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 16 Oct 2021 12:24:41 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 16 Oct 2021 12:24:42 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Oct 2021 12:24:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 16 Oct 2021 12:24:44 GMT
WORKDIR /usr/local/tomcat
# Sat, 16 Oct 2021 12:24:45 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 16 Oct 2021 12:24:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 16 Oct 2021 12:37:23 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 16 Oct 2021 12:37:24 GMT
ENV TOMCAT_MAJOR=9
# Sat, 16 Oct 2021 12:37:25 GMT
ENV TOMCAT_VERSION=9.0.54
# Sat, 16 Oct 2021 12:37:26 GMT
ENV TOMCAT_SHA512=83430f24d42186ce2ff51eeef2f7a5517048f37d9050c45cac1e3dba8926d61a1f7f5aba122a34a11ac1dbdd3c1f6d98671841047df139394d43751263de57c3
# Sat, 16 Oct 2021 12:37:28 GMT
COPY dir:afa0755983a007414ccf98ebed8d81729d86baf9f7bad4d08e8a32bfb01b80b9 in /usr/local/tomcat 
# Sat, 16 Oct 2021 12:37:31 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 12:37:32 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 16 Oct 2021 12:37:33 GMT
EXPOSE 8080
# Sat, 16 Oct 2021 12:37:34 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1c47a423366578e5ce665d03788914bf0459485a627a27896fa9c5663ce55cdf`  
		Last Modified: Tue, 12 Oct 2021 01:47:41 GMT  
		Size: 53.6 MB (53603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b1f128be8ebd64f787c46418ffe34ce1096d1ccd6938924d7397713720758`  
		Last Modified: Sat, 16 Oct 2021 03:14:21 GMT  
		Size: 5.1 MB (5141861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c338d42ad921985fb8ebb6e2c48d381f6e03a91535eeffce7f08084b3dfbfdf4`  
		Last Modified: Sat, 16 Oct 2021 03:14:21 GMT  
		Size: 10.7 MB (10655847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc106854165a44e13d4168fd90671d6e4b959240373bf60b731fe8b7d01123`  
		Last Modified: Sat, 16 Oct 2021 04:29:12 GMT  
		Size: 5.6 MB (5647129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd97a334a10820fa2c4db4cf880785991c2de11ad0b9566bf2ca80bfb1ef356`  
		Last Modified: Sat, 16 Oct 2021 04:31:06 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bb12b18bc137ea3bbb1fc3c5fc731a5be31bf85f7e0105f0fdd0f1ba11829a`  
		Last Modified: Sat, 16 Oct 2021 04:31:13 GMT  
		Size: 40.6 MB (40615174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bb4a7b24dd3c496a50eced03924d5178c04b15188d3d542f499ff806c06342`  
		Last Modified: Sat, 16 Oct 2021 13:27:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d83302074f131e00c8846e35cc6940846f8db945dd30e43e7d2165215c139d6`  
		Last Modified: Sat, 16 Oct 2021 13:36:39 GMT  
		Size: 12.2 MB (12164950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc4531bada1bccdd29c8539e0f07b5bc385685549390f05d745194d81af7cfb`  
		Last Modified: Sat, 16 Oct 2021 13:36:38 GMT  
		Size: 217.0 KB (216962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
