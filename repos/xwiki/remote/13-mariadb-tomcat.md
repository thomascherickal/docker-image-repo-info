## `xwiki:13-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:414a15dce7aceb69b0eceee773b884e9c9c7ea3eaa70b74be573c89a322fec68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:13-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5bf9ace8277a54f1879e1a11c126d5298037f2e6d44500bd9e7fd3da676c0d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **628.5 MB (628487539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad0e124a29f8d8cf9ac42a94f55fe36574547748c8891eb8b5164c51e273c4ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:48:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 15:47:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:47:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Jul 2022 15:47:29 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Jul 2022 15:47:29 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 15:47:29 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 20:28:07 GMT
ENV JAVA_VERSION=11.0.16
# Mon, 25 Jul 2022 20:28:14 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_11.0.16_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_11.0.16_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Mon, 25 Jul 2022 23:09:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 25 Jul 2022 23:09:40 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Jul 2022 23:09:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 25 Jul 2022 23:09:41 GMT
WORKDIR /usr/local/tomcat
# Mon, 25 Jul 2022 23:09:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 25 Jul 2022 23:09:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 25 Jul 2022 23:16:18 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 25 Jul 2022 23:16:18 GMT
ENV TOMCAT_MAJOR=9
# Mon, 25 Jul 2022 23:16:18 GMT
ENV TOMCAT_VERSION=9.0.65
# Mon, 25 Jul 2022 23:16:18 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Mon, 25 Jul 2022 23:16:19 GMT
COPY dir:72a6b2f810555478cfa1d75e94ad553add3571bc6014f31867f07702411cbb5a in /usr/local/tomcat 
# Mon, 25 Jul 2022 23:16:23 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 25 Jul 2022 23:16:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 25 Jul 2022 23:16:24 GMT
EXPOSE 8080
# Mon, 25 Jul 2022 23:16:24 GMT
CMD ["catalina.sh" "run"]
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 26 Jul 2022 00:51:35 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 26 Jul 2022 00:52:12 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 18:46:20 GMT
ENV XWIKI_VERSION=13.10.8
# Wed, 27 Jul 2022 18:46:20 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.8
# Wed, 27 Jul 2022 18:46:20 GMT
ENV XWIKI_DOWNLOAD_SHA256=d6da0bdfb5e0c9e5acccd13a9ff2d40a5bda2a3f9db4426f58fe8f47c262f4b7
# Wed, 27 Jul 2022 18:46:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 27 Jul 2022 18:47:56 GMT
ENV MARIADB_JDBC_VERSION=3.0.6
# Wed, 27 Jul 2022 18:47:57 GMT
ENV MARIADB_JDBC_SHA256=977ca7980b777b5aa8d32678204296a108f3eacbc4f210887e39b19869fad0d3
# Wed, 27 Jul 2022 18:47:57 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.0.6
# Wed, 27 Jul 2022 18:47:57 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.0.6.jar
# Wed, 27 Jul 2022 18:47:57 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.0.6.jar
# Wed, 27 Jul 2022 18:47:58 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 27 Jul 2022 18:47:58 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 27 Jul 2022 18:47:58 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 27 Jul 2022 18:47:58 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 27 Jul 2022 18:47:59 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 27 Jul 2022 18:47:59 GMT
VOLUME [/usr/local/xwiki]
# Wed, 27 Jul 2022 18:47:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Jul 2022 18:47:59 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a9e63c657ad881997f5165c0826be395bfc064415876b9fbaae74bcb5dc721`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 5.2 MB (5156110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1989b6e74cfdda1591b9dd23be47c5caeb002b7a151379361ec0c3f0e6d0e52`  
		Last Modified: Tue, 12 Jul 2022 02:55:03 GMT  
		Size: 10.9 MB (10876416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19babefbed0663644efc4f2bc7bc5ae6914628808e42cd7dae490844da02ef4a`  
		Last Modified: Tue, 12 Jul 2022 16:00:07 GMT  
		Size: 5.7 MB (5657891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529e95713a10aa41fdb7a9f2a610a4c32b721b77d74f3c1e6aadec5170a893db`  
		Last Modified: Tue, 12 Jul 2022 16:00:06 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956f2f36dfb2b2629ab92608a3737feb92c98d7bd4ad40a6e2820362bd32e66b`  
		Last Modified: Mon, 25 Jul 2022 20:40:50 GMT  
		Size: 45.8 MB (45769248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af8fbbe689577d47ddbb27e4fe4b72d10454452e8ba2a0c0ae2039c645c0d93`  
		Last Modified: Mon, 25 Jul 2022 23:37:54 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1844fc3636b7287f28031d80db992be8b8aca238a3221229d30973abd3b8770`  
		Last Modified: Mon, 25 Jul 2022 23:44:24 GMT  
		Size: 12.2 MB (12160309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b948b6d231d0d8e60eb07f8df5bebe5e6b4161ce58c5b12eb8a4f798c9da9a`  
		Last Modified: Mon, 25 Jul 2022 23:44:23 GMT  
		Size: 459.7 KB (459730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71387be9557aa79eb3d963fa85977a78e812ecb9a5fba842f16c38703776961`  
		Last Modified: Mon, 25 Jul 2022 23:44:23 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac69536873246f7a29ea24de2b90a0182b0ecad61505d0005b7bc7f796e11e1f`  
		Last Modified: Tue, 26 Jul 2022 00:59:15 GMT  
		Size: 200.2 MB (200196648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec91fbb03951c7ec304065eacf333012a7921511c6bc586044dcd40d1b37d670`  
		Last Modified: Wed, 27 Jul 2022 18:49:20 GMT  
		Size: 292.7 MB (292658658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be40e66d0e5f35b8f8f4a5878329c12cd5d35e1c0de85550bf182be7327ddd1`  
		Last Modified: Wed, 27 Jul 2022 18:50:36 GMT  
		Size: 541.1 KB (541127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddde2b11615dd2a564987833c33d238b740bea0c9fd27137a3d7dbf85af18c67`  
		Last Modified: Wed, 27 Jul 2022 18:50:35 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9323a0549bef2ca1c295993007f8d41c08f1577eff2f5e0a369fee4dbc0dab`  
		Last Modified: Wed, 27 Jul 2022 18:50:35 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77bd4a9c9650d9d8dcce6c21f12c5ae1eb44236d60b3a7261dbfb361c31fafe`  
		Last Modified: Wed, 27 Jul 2022 18:50:35 GMT  
		Size: 5.3 KB (5331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc85cef06b29d838b7f934fc26d51c95f295363f072e50d50142701741022f27`  
		Last Modified: Wed, 27 Jul 2022 18:50:35 GMT  
		Size: 2.5 KB (2503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:13-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:8a56c7829843d00a6b7b720ea4f0da9b2196f566f5ce4be8018d79474126984f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.0 MB (621025435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82f527c437c31b5898e3e2ba65368c7024f19d67de4c2d39c4a0274d3966e57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:18 GMT
ADD file:2dcc013bca5a420cad3b6a1ac61f52ea58a29ae05fe282078a744979c0e1a89e in / 
# Tue, 12 Jul 2022 00:40:19 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:33:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 16:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 16:45:16 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Jul 2022 16:45:17 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Jul 2022 16:45:18 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jul 2022 16:45:19 GMT
ENV LANG=C.UTF-8
# Mon, 25 Jul 2022 20:55:16 GMT
ENV JAVA_VERSION=11.0.16
# Mon, 25 Jul 2022 20:55:24 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_11.0.16_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_11.0.16_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Mon, 25 Jul 2022 22:46:32 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 25 Jul 2022 22:46:33 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 25 Jul 2022 22:46:34 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 25 Jul 2022 22:46:35 GMT
WORKDIR /usr/local/tomcat
# Mon, 25 Jul 2022 22:46:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 25 Jul 2022 22:46:37 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 25 Jul 2022 22:57:24 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 25 Jul 2022 22:57:25 GMT
ENV TOMCAT_MAJOR=9
# Mon, 25 Jul 2022 22:57:26 GMT
ENV TOMCAT_VERSION=9.0.65
# Mon, 25 Jul 2022 22:57:27 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Mon, 25 Jul 2022 22:57:29 GMT
COPY dir:059248f08f53074e1160790c44bfa2640b6ff7900afa307c184717fd1cafda65 in /usr/local/tomcat 
# Mon, 25 Jul 2022 22:57:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 25 Jul 2022 22:57:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 25 Jul 2022 22:57:34 GMT
EXPOSE 8080
# Mon, 25 Jul 2022 22:57:35 GMT
CMD ["catalina.sh" "run"]
# Tue, 26 Jul 2022 01:35:13 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 26 Jul 2022 01:35:14 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 26 Jul 2022 01:35:15 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 26 Jul 2022 01:35:16 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 26 Jul 2022 01:35:17 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 26 Jul 2022 01:35:18 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 26 Jul 2022 01:35:49 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 01:40:10 GMT
ENV XWIKI_VERSION=13.10.7
# Tue, 26 Jul 2022 01:40:11 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.7
# Tue, 26 Jul 2022 01:40:11 GMT
ENV XWIKI_DOWNLOAD_SHA256=b886e886ed34e8d7bea8feb2e74e94edb3fb88030f90ab68c7bbc87dcf453d00
# Tue, 26 Jul 2022 01:40:46 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 26 Jul 2022 01:42:04 GMT
ENV MARIADB_JDBC_VERSION=3.0.6
# Tue, 26 Jul 2022 01:42:05 GMT
ENV MARIADB_JDBC_SHA256=977ca7980b777b5aa8d32678204296a108f3eacbc4f210887e39b19869fad0d3
# Tue, 26 Jul 2022 01:42:06 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.0.6
# Tue, 26 Jul 2022 01:42:07 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.0.6.jar
# Tue, 26 Jul 2022 01:42:07 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.0.6.jar
# Tue, 26 Jul 2022 01:42:09 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 26 Jul 2022 01:42:10 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 26 Jul 2022 01:42:11 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 26 Jul 2022 01:42:12 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 26 Jul 2022 01:42:13 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 26 Jul 2022 01:42:13 GMT
VOLUME [/usr/local/xwiki]
# Tue, 26 Jul 2022 01:42:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 01:42:15 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:cfc947b533a3ed8b8ce79820c7fe5e7634bf9c08479ed0aee1e74ee7b4f2b068`  
		Last Modified: Tue, 12 Jul 2022 00:45:41 GMT  
		Size: 53.7 MB (53683129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca36aa4204d2a708dcd1d41d1d4a128b095f8d88a2f9544f89799c36914e356`  
		Last Modified: Tue, 12 Jul 2022 02:42:29 GMT  
		Size: 5.1 MB (5142960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdcd2014de70fbce8c43a70cd1f42bceab4f1e35953db987fc318dbc0fb0d26`  
		Last Modified: Tue, 12 Jul 2022 02:42:30 GMT  
		Size: 10.7 MB (10657500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60047e9914e670a899370adf2dd0fa2454a135151f9b3a2b871f18ef9e193bce`  
		Last Modified: Tue, 12 Jul 2022 17:04:52 GMT  
		Size: 5.6 MB (5648704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe81dbfbe8d8bda9067737340106f1de9bfae84dda03edf2640783c25345ef2`  
		Last Modified: Tue, 12 Jul 2022 17:04:51 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f4917b3a622c1c72fd6a59682fa52c5a46bf90a7bc937b7f8afad2ec042eab`  
		Last Modified: Mon, 25 Jul 2022 21:13:48 GMT  
		Size: 45.1 MB (45070702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87024ffaf0ab687ff6650d13cce94086f1e6cd57203cf5b360662075b44ea15`  
		Last Modified: Mon, 25 Jul 2022 23:33:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eeeb39db3196d973fb6052926704560265ba85b7c85cc7a91c8030d715ae919`  
		Last Modified: Mon, 25 Jul 2022 23:40:57 GMT  
		Size: 12.2 MB (12170160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c43e8ed3866c54c631cc08e4b743a9c562954a155f030547435d747ba1a5cd`  
		Last Modified: Mon, 25 Jul 2022 23:40:56 GMT  
		Size: 217.2 KB (217196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02850df55f43c178242804a93e72d37887d710185bf3478a17e9ddbd5e165937`  
		Last Modified: Tue, 26 Jul 2022 01:44:20 GMT  
		Size: 195.2 MB (195240641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efea34ae25debf086c3c946d2aae72d2e8d9abf2a41105d3f012fc0e8939b91`  
		Last Modified: Tue, 26 Jul 2022 01:48:26 GMT  
		Size: 292.6 MB (292641473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19915b0867b6fa08970ce37bfa9661c513861afc054c7154e18dccbe8e1917d3`  
		Last Modified: Tue, 26 Jul 2022 01:49:54 GMT  
		Size: 541.1 KB (541129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0efa1a9dbb65a4e0d852bd0fa38075333d80b2cc3b1559e0b1dd23d429891`  
		Last Modified: Tue, 26 Jul 2022 01:49:53 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd622f2a880513074379fc7b7976f124b3dc96462d687b0e23c14ca76d799a`  
		Last Modified: Tue, 26 Jul 2022 01:49:53 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba84529eac3be98351ec3771de7e86f88519e0f69b60eb70d908f38fe7d38e9`  
		Last Modified: Tue, 26 Jul 2022 01:49:53 GMT  
		Size: 5.3 KB (5335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7004ff8b7ca9963cd53c9cdc5da059f00fa4cfa3324f358015ca3d60e57e1d1a`  
		Last Modified: Tue, 26 Jul 2022 01:49:53 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
