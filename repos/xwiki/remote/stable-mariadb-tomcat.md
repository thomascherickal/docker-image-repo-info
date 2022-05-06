## `xwiki:stable-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:84b6705a20f683ceec6b2918276275c39fa58115d6229c2df06e5214d3a7aec6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f97ac2ee9c3724bd2459b231c33ed53e14b9972ec0590e331e950bd1b10f14c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **629.1 MB (629102352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23aa6b85892099b7723d53014ea3959bd87ad6c506bc4183682e0f466a7ae2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:53:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 20 Apr 2022 10:53:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 20 Apr 2022 10:53:58 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:53:58 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:27:13 GMT
ENV JAVA_VERSION=11.0.15
# Mon, 25 Apr 2022 18:27:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Mon, 25 Apr 2022 21:58:01 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 25 Apr 2022 21:58:01 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Apr 2022 21:58:02 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 25 Apr 2022 21:58:02 GMT
WORKDIR /usr/local/tomcat
# Mon, 25 Apr 2022 21:58:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 25 Apr 2022 21:58:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 25 Apr 2022 22:05:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 25 Apr 2022 22:05:04 GMT
ENV TOMCAT_MAJOR=9
# Mon, 25 Apr 2022 22:05:04 GMT
ENV TOMCAT_VERSION=9.0.62
# Mon, 25 Apr 2022 22:05:04 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Mon, 25 Apr 2022 22:05:05 GMT
COPY dir:95b8a3ec00ea840c59bd0e77b3998ce0f4d0a237879ba7ddad322b7a1ee96f62 in /usr/local/tomcat 
# Mon, 25 Apr 2022 22:05:08 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 22:05:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 25 Apr 2022 22:05:09 GMT
EXPOSE 8080
# Mon, 25 Apr 2022 22:05:09 GMT
CMD ["catalina.sh" "run"]
# Fri, 06 May 2022 19:27:12 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 06 May 2022 19:27:13 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 06 May 2022 19:27:13 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 06 May 2022 19:27:13 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 06 May 2022 19:27:13 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 06 May 2022 19:27:13 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 06 May 2022 19:27:51 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 06 May 2022 19:27:52 GMT
ENV XWIKI_VERSION=14.3.1
# Fri, 06 May 2022 19:27:52 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.3.1
# Fri, 06 May 2022 19:27:52 GMT
ENV XWIKI_DOWNLOAD_SHA256=48555f31d174709b5eb8486204fbbdfc51fbbda17cb28d8bf5ac8551f3f9820b
# Fri, 06 May 2022 19:28:30 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 06 May 2022 19:30:00 GMT
ENV MARIADB_JDBC_VERSION=3.0.4
# Fri, 06 May 2022 19:30:00 GMT
ENV MARIADB_JDBC_SHA256=c8c9eba4f5368e3fdb321e17353446cbf8d36c822ec604841308b1bef950a529
# Fri, 06 May 2022 19:30:00 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.0.4
# Fri, 06 May 2022 19:30:00 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.0.4.jar
# Fri, 06 May 2022 19:30:00 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.0.4.jar
# Fri, 06 May 2022 19:30:01 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Fri, 06 May 2022 19:30:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 06 May 2022 19:30:01 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 06 May 2022 19:30:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 06 May 2022 19:30:02 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 06 May 2022 19:30:02 GMT
VOLUME [/usr/local/xwiki]
# Fri, 06 May 2022 19:30:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 May 2022 19:30:02 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ccb680c1c472c36a4595e2d4a2b4d1a434c377feb1ec57942b4006051064e6`  
		Last Modified: Wed, 20 Apr 2022 11:12:20 GMT  
		Size: 5.7 MB (5657427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c2d2d2ad823b35ca184fcea252da3e7848e1ed4b31168688a265e4a1ab86b0`  
		Last Modified: Wed, 20 Apr 2022 11:12:19 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa59d9ab33cd135fc03bd1449112beaf19d1eb922727cb5c81008ff68b12f95`  
		Last Modified: Mon, 25 Apr 2022 18:41:27 GMT  
		Size: 47.2 MB (47197425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6bf2afbce219c39dc09163d437e53379070254ab1421e85a4a59afc912d6f8`  
		Last Modified: Mon, 25 Apr 2022 22:21:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f96426cd061ed80020e30ae9d37d5e9d2623a2ef4eff2ec824ea979573de9`  
		Last Modified: Tue, 26 Apr 2022 00:09:25 GMT  
		Size: 12.1 MB (12141236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d14afebc09c8540ff38d1ffa033ace23c0d4157051f7ae5a5ede6d6eaf97d7`  
		Last Modified: Tue, 26 Apr 2022 00:09:25 GMT  
		Size: 459.6 KB (459626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab470316cc6b04b95bac9ac28cb438f957362db0b1ce01f6624596a3f351cfb1`  
		Last Modified: Tue, 26 Apr 2022 00:09:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd32f0d7ce5249a3a2ec13f7ac5aef9d9650143933c6eb15f64f49fad78f567`  
		Last Modified: Fri, 06 May 2022 19:31:20 GMT  
		Size: 200.2 MB (200196708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06fa825ff1020bf2ba869634642a875fe8d13b3e96b5c30a11e908868f09731`  
		Last Modified: Fri, 06 May 2022 19:31:09 GMT  
		Size: 291.9 MB (291936710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed122ec3792529fcb39400472bd03275ecf5ca32c5c79ec26be8b47e6f3f8231`  
		Last Modified: Fri, 06 May 2022 19:32:55 GMT  
		Size: 528.3 KB (528299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47af455455984d0b5640dc44729cf8c7281ae7cab08083c0ea26a0bec70ea21`  
		Last Modified: Fri, 06 May 2022 19:32:55 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becabb58ed79ea8000fac2e30035755d316a21e989a1803808b8234630621a08`  
		Last Modified: Fri, 06 May 2022 19:32:55 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f0b56cf7dd299a1ad1bac5db250c266b16856148f6413897a196d824722362`  
		Last Modified: Fri, 06 May 2022 19:32:55 GMT  
		Size: 5.8 KB (5839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7101d7d2aadfb728c1a972299619136586413ef17c60cc8b46dce0a671d6625`  
		Last Modified: Fri, 06 May 2022 19:32:55 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:f12246505fd19c5120ee26a3ba6b155014fd738260c40113e1e5191b56adb7f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.5 MB (621469923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36b48a9bc30e95199a394e808c6dfa244be7f1b11b01b95f95fe5e5ba9ca76c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:33:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:33:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 20 Apr 2022 10:33:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 20 Apr 2022 10:33:23 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:33:24 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:47:08 GMT
ENV JAVA_VERSION=11.0.15
# Mon, 25 Apr 2022 18:47:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Mon, 25 Apr 2022 23:18:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 25 Apr 2022 23:18:49 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Apr 2022 23:18:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 25 Apr 2022 23:18:51 GMT
WORKDIR /usr/local/tomcat
# Mon, 25 Apr 2022 23:18:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 25 Apr 2022 23:18:53 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 25 Apr 2022 23:30:35 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 25 Apr 2022 23:30:36 GMT
ENV TOMCAT_MAJOR=9
# Mon, 25 Apr 2022 23:30:37 GMT
ENV TOMCAT_VERSION=9.0.62
# Mon, 25 Apr 2022 23:30:38 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Mon, 25 Apr 2022 23:30:40 GMT
COPY dir:7d7624ba066b1a2d857646a8679cc71837d600696d37c7a2519b0ed9fa234a97 in /usr/local/tomcat 
# Mon, 25 Apr 2022 23:30:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 23:30:45 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 25 Apr 2022 23:30:46 GMT
EXPOSE 8080
# Mon, 25 Apr 2022 23:30:47 GMT
CMD ["catalina.sh" "run"]
# Fri, 06 May 2022 19:41:25 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 06 May 2022 19:41:25 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 06 May 2022 19:41:26 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 06 May 2022 19:41:27 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 06 May 2022 19:41:28 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 06 May 2022 19:41:29 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 06 May 2022 19:42:12 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 06 May 2022 19:42:13 GMT
ENV XWIKI_VERSION=14.3.1
# Fri, 06 May 2022 19:42:14 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.3.1
# Fri, 06 May 2022 19:42:15 GMT
ENV XWIKI_DOWNLOAD_SHA256=48555f31d174709b5eb8486204fbbdfc51fbbda17cb28d8bf5ac8551f3f9820b
# Fri, 06 May 2022 19:42:40 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 06 May 2022 19:44:34 GMT
ENV MARIADB_JDBC_VERSION=3.0.4
# Fri, 06 May 2022 19:44:35 GMT
ENV MARIADB_JDBC_SHA256=c8c9eba4f5368e3fdb321e17353446cbf8d36c822ec604841308b1bef950a529
# Fri, 06 May 2022 19:44:36 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.0.4
# Fri, 06 May 2022 19:44:36 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.0.4.jar
# Fri, 06 May 2022 19:44:37 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.0.4.jar
# Fri, 06 May 2022 19:44:39 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Fri, 06 May 2022 19:44:40 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 06 May 2022 19:44:41 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 06 May 2022 19:44:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 06 May 2022 19:44:43 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 06 May 2022 19:44:44 GMT
VOLUME [/usr/local/xwiki]
# Fri, 06 May 2022 19:44:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 May 2022 19:44:45 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579ba6ed012bb5067169efabd19955cc8bc89ef5df54b8aac8fa222e892c1e88`  
		Last Modified: Wed, 20 Apr 2022 10:58:19 GMT  
		Size: 5.6 MB (5649495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46016f3a0b390c1ffbf70f7c3608b0562ff1162909dac20f2e3cf144104f0ac4`  
		Last Modified: Wed, 20 Apr 2022 10:58:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f71d741c3da5bc68e593fc3090ef28cf8e5959d3b2c90ab8513676d94d7b69`  
		Last Modified: Mon, 25 Apr 2022 19:07:48 GMT  
		Size: 46.5 MB (46498865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be97b6364dd9adfda457a03afcfc3e09566dc0a7e144e7adf881d88812fda86`  
		Last Modified: Tue, 26 Apr 2022 00:00:12 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ca98c3627dde38d3159a2f91a71c6da7ac70ab051bb983868e469c3e6c119b`  
		Last Modified: Tue, 26 Apr 2022 00:10:08 GMT  
		Size: 12.2 MB (12150082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8931b623547de21bbf248c9449694007c8c9bd8e806dfa47c83654a2ebf8a9`  
		Last Modified: Tue, 26 Apr 2022 00:10:07 GMT  
		Size: 217.2 KB (217155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c8d3f77440a3f9d47b7ed501e27be7a8374ad5ecaf3e342fd4f691af05e6b9`  
		Last Modified: Fri, 06 May 2022 19:46:57 GMT  
		Size: 195.2 MB (195248291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb312976869012c4148a1b2c835b3a9b3a723bb172bf48558190114b0f0fb22`  
		Last Modified: Fri, 06 May 2022 19:46:51 GMT  
		Size: 291.9 MB (291936671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f85acae4e9503c4f6be84ac8786f6d74029da9ab4f5338b1cee6129ab295f71`  
		Last Modified: Fri, 06 May 2022 19:48:39 GMT  
		Size: 528.3 KB (528294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecd23fd8ec8f309b75be663a25d50f43aafac4e0519a96573ab75e8ead04668`  
		Last Modified: Fri, 06 May 2022 19:48:39 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423bcb0e59e49aaf0d702b24c842aa8142d8ff364e0cab5e4c61c087061f1116`  
		Last Modified: Fri, 06 May 2022 19:48:39 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3e18ab5af7d5228f8e48f68625abb2ac730113287269d9cc3752d2ea61790a`  
		Last Modified: Fri, 06 May 2022 19:48:39 GMT  
		Size: 5.8 KB (5841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0081c5d8c009e49113272f3d5b069ceeb2d5618bafed849729a7677d290a04f5`  
		Last Modified: Fri, 06 May 2022 19:48:39 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
