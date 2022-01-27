## `tomcat:10-jre11-openjdk-buster`

```console
$ docker pull tomcat@sha256:aaa774454b1055727052f28f469f69ad4f2b9c515147d8b6982c373fd6ac07ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jre11-openjdk-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:20f72cdc0237c8dc4a0233e40394cde47b7c39e746849618698aa2c03b1ec9c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133649828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690b936be732ba4e03ac0ca73cdae665acc92940faa00140104be04323477057`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:05:25 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 21 Dec 2021 23:05:26 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:05:26 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:05:26 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:05:27 GMT
ENV JAVA_VERSION=11.0.13
# Tue, 21 Dec 2021 23:05:37 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 22 Dec 2021 17:02:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:02:15 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:02:16 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:02:16 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:02:16 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:02:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:02:17 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 22 Dec 2021 17:02:17 GMT
ENV TOMCAT_MAJOR=10
# Fri, 21 Jan 2022 01:47:07 GMT
ENV TOMCAT_VERSION=10.0.16
# Fri, 21 Jan 2022 01:47:07 GMT
ENV TOMCAT_SHA512=9b70f4db2c7b2efb5453cd581322b1137df7b6443acd6a8e278eaaf97de89c9ad0c7c7996a2d545ef1e4d965aca43c40d2b2c7d5e46b021695f87093143fbba2
# Fri, 21 Jan 2022 01:47:08 GMT
COPY dir:1c1681a1bd927cb6a2fc9f5d870210ad30bbaa5d0e78f1dc587f0d5539552fd1 in /usr/local/tomcat 
# Fri, 21 Jan 2022 01:47:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:47:14 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 01:47:14 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 01:47:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2660882c117d85771a35a9eea4575a40aa99860ff668bc820cb7aec845bc06e`  
		Last Modified: Tue, 21 Dec 2021 23:27:02 GMT  
		Size: 5.5 MB (5531115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda90940f92391d3f723301da3b6a68a0486304439e39e97be9b3dedf4227337`  
		Last Modified: Tue, 21 Dec 2021 23:27:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88ce3eec0de41956fdd09e02fb156c42381d438a425623ddbf8133926fe288`  
		Last Modified: Tue, 21 Dec 2021 23:27:10 GMT  
		Size: 46.8 MB (46841172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfb800f91fde218e41a99486412f2103f5482ce916fc3b90d8f4de3501e3ca8`  
		Last Modified: Wed, 22 Dec 2021 17:44:24 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27613478db209a48b8e5adffe63421d0189a3797e63a911a78fab956095be625`  
		Last Modified: Fri, 21 Jan 2022 02:50:40 GMT  
		Size: 12.5 MB (12547886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d60b34c6fc2c95d1ad83b9730fbb4f9e86476c0bce9dc79fdb32074fd8e8685`  
		Last Modified: Fri, 21 Jan 2022 02:50:39 GMT  
		Size: 461.0 KB (460970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0b846488ae80606c7cf03d68cc90a49554b79873f50dbbe5c0fcd18780cf6a`  
		Last Modified: Fri, 21 Jan 2022 02:50:38 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre11-openjdk-buster` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:12c4ad2f1665f4d34f81432e7f90cb0c862c921a622d96ba36de92dbe850b353
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130898392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7ab43c0ca77e9c013453fefdc512092087ae3f27733a4799b9c5dc5f2af6ed`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:41 GMT
ADD file:98a75269e438ff15cee16ad2763fe2698fb436bc4770c0ca27c059f66b65e56a in / 
# Wed, 26 Jan 2022 01:42:42 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:14:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 06:00:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:00:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Jan 2022 06:00:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:00:03 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:00:04 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 06:00:05 GMT
ENV JAVA_VERSION=11.0.13
# Wed, 26 Jan 2022 06:00:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Wed, 26 Jan 2022 23:47:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Jan 2022 23:47:56 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 23:47:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Jan 2022 23:47:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Jan 2022 23:47:59 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jan 2022 23:48:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jan 2022 23:48:01 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Jan 2022 23:48:02 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Jan 2022 23:56:15 GMT
ENV TOMCAT_VERSION=10.0.16
# Wed, 26 Jan 2022 23:56:15 GMT
ENV TOMCAT_SHA512=9b70f4db2c7b2efb5453cd581322b1137df7b6443acd6a8e278eaaf97de89c9ad0c7c7996a2d545ef1e4d965aca43c40d2b2c7d5e46b021695f87093143fbba2
# Wed, 26 Jan 2022 23:56:17 GMT
COPY dir:92e4e55da7edfd8810cf98101f18a725566505abbf816ffc720cb77fc65e96d4 in /usr/local/tomcat 
# Wed, 26 Jan 2022 23:56:20 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 23:56:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Jan 2022 23:56:23 GMT
EXPOSE 8080
# Wed, 26 Jan 2022 23:56:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ccd458f933f7966e412773ee1551aaf2433a5bf9adaae519e2ac7c9c3f8b5f89`  
		Last Modified: Wed, 26 Jan 2022 01:49:28 GMT  
		Size: 49.2 MB (49223041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3524e6d2c855bef1f32da73e00738b2e5e91e6a346d19f8b33e8e8117c82748`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 7.7 MB (7695112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc9cf00cd9023559aeda43668c7d9d621318631bab103ae03b8a3787260048`  
		Last Modified: Wed, 26 Jan 2022 02:25:05 GMT  
		Size: 9.8 MB (9767300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb47824c903cca25cdc9a24eb3596e18ae0d673921bb6c79164a4ce0317c77`  
		Last Modified: Wed, 26 Jan 2022 06:27:25 GMT  
		Size: 5.5 MB (5505341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e66059e0d74af6d8ea2767ddeb4ffda8df4f462807adedc4c43042ecc1b83fd`  
		Last Modified: Wed, 26 Jan 2022 06:27:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2384e75f09bba0668d56a2eb286e4c8ac3ec0cf40f354e873d02c5ff91a6b8bf`  
		Last Modified: Wed, 26 Jan 2022 06:27:31 GMT  
		Size: 45.9 MB (45927634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d65badfd191f7458fc6906b51445410d56fa5dacef077f1b1106d0a97ad00`  
		Last Modified: Thu, 27 Jan 2022 00:50:24 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41837f152d5ce8a3db2e0486d9bca101e1198db73d28aaeb3eaf5b1fb38ec55c`  
		Last Modified: Thu, 27 Jan 2022 00:56:26 GMT  
		Size: 12.6 MB (12561397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9bd98d0104fe373018a23eb995c4d1b26dda6f55a8d977f6617dd35b21bfc2`  
		Last Modified: Thu, 27 Jan 2022 00:56:24 GMT  
		Size: 218.2 KB (218216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
