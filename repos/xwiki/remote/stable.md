## `xwiki:stable`

```console
$ docker pull xwiki@sha256:ee11f89031b73c8362981786e7a55f7ff1190da2c6ebb8abc158c36949ebc49a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable` - linux; amd64

```console
$ docker pull xwiki@sha256:85dd957341f79eedd319a0c2f4af6bf61f49c4c3a50a8d629fb353ff1691d0a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **631.1 MB (631060787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76f83a119d1d3c1bd6448898bde9a1803cb343a20489b8da69f8b6ee90aaaa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:40:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:40:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 19:38:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 19:38:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 May 2022 19:38:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Sat, 28 May 2022 19:38:32 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 19:38:32 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 19:38:33 GMT
ENV JAVA_VERSION=11.0.15
# Sat, 28 May 2022 19:38:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Sat, 28 May 2022 21:45:47 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 28 May 2022 21:45:47 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 21:45:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 28 May 2022 21:45:47 GMT
WORKDIR /usr/local/tomcat
# Sat, 28 May 2022 21:45:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 28 May 2022 21:45:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 28 May 2022 21:54:48 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 28 May 2022 21:54:48 GMT
ENV TOMCAT_MAJOR=9
# Sat, 28 May 2022 21:54:48 GMT
ENV TOMCAT_VERSION=9.0.63
# Sat, 28 May 2022 21:54:48 GMT
ENV TOMCAT_SHA512=4b905018164026756bd36ab9fde8f6b21c886acb8e5255d93f8938491e4d375dd18b9fc58ee23e3d78b16e8b81271c1c998e5592beedcac632567c2ca9411c69
# Sat, 28 May 2022 21:54:48 GMT
COPY dir:8c17847f7db73ee77738efc7d78cd9afc7b32296a7e53c3e15448c21f97c623e in /usr/local/tomcat 
# Sat, 28 May 2022 21:54:52 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 21:54:53 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 28 May 2022 21:54:53 GMT
EXPOSE 8080
# Sat, 28 May 2022 21:54:53 GMT
CMD ["catalina.sh" "run"]
# Sun, 29 May 2022 05:30:32 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sun, 29 May 2022 05:30:32 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sun, 29 May 2022 05:30:32 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sun, 29 May 2022 05:30:33 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sun, 29 May 2022 05:30:33 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sun, 29 May 2022 05:30:33 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sun, 29 May 2022 05:31:11 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 05:31:13 GMT
ENV XWIKI_VERSION=14.4
# Sun, 29 May 2022 05:31:13 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.4
# Sun, 29 May 2022 05:31:13 GMT
ENV XWIKI_DOWNLOAD_SHA256=313983ea4e1c8f7f44058bedf150e61b9b57a0a9c00c99b3a6471a4f567010e3
# Sun, 29 May 2022 05:31:51 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sun, 29 May 2022 05:31:51 GMT
ENV MYSQL_JDBC_VERSION=8.0.29
# Sun, 29 May 2022 05:31:52 GMT
ENV MYSQL_JDBC_SHA256=d4e32d2a6026b5acc00300b73a86c28fb92681ae9629b21048ee67014c911db6
# Sun, 29 May 2022 05:31:52 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.29
# Sun, 29 May 2022 05:31:52 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.29.jar
# Sun, 29 May 2022 05:31:52 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.29.jar
# Sun, 29 May 2022 05:31:53 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sun, 29 May 2022 05:31:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sun, 29 May 2022 05:31:53 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sun, 29 May 2022 05:31:53 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sun, 29 May 2022 05:31:53 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sun, 29 May 2022 05:31:53 GMT
VOLUME [/usr/local/xwiki]
# Sun, 29 May 2022 05:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 05:31:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf168a6748997eb97b48cc86234b7ff7d8bc907645b9be99013158b3f146b272`  
		Last Modified: Sat, 28 May 2022 02:49:08 GMT  
		Size: 5.2 MB (5156036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e604223835ccf02d097187b5a58ca73e8598cadbb16a36202ca1943e97f56f1f`  
		Last Modified: Sat, 28 May 2022 02:49:08 GMT  
		Size: 10.9 MB (10875008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879d05afe7d1ed6ac0f5b2d9537450b8058210d5c1ba04e3dbdfd0ea7f44da0`  
		Last Modified: Sat, 28 May 2022 19:48:32 GMT  
		Size: 5.7 MB (5657595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67409f01891c54bb4d7cf58512ec5cef2762ae616c2ab81d132c671c585f27b4`  
		Last Modified: Sat, 28 May 2022 19:48:31 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777f3575eb5979e51c7805e2bf9b825868bbd06f981240a48991e55828c1f206`  
		Last Modified: Sat, 28 May 2022 19:48:38 GMT  
		Size: 47.2 MB (47197487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b03265e3e87ebc901b1160b3b4f25f1e477105358369d25546a30af93d003c`  
		Last Modified: Sat, 28 May 2022 22:14:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98448e1908d9b7f20e4c7192091b6b0a140caea46dacedb799ae36e315f03f5c`  
		Last Modified: Sat, 28 May 2022 22:24:33 GMT  
		Size: 12.1 MB (12149608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b074305b7917ecc1cf519ac07a6683163948f783f886d81458b63e443ea9665`  
		Last Modified: Sat, 28 May 2022 22:24:32 GMT  
		Size: 459.7 KB (459743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f278316e469eba5f92efe6cbaa20b033ac3398f95258be91ace48e8a4e787e8`  
		Last Modified: Sat, 28 May 2022 22:24:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1db49372ab6440b3021006c4a8855382515ee9296a94fc153c913c07277556e`  
		Last Modified: Sun, 29 May 2022 05:36:31 GMT  
		Size: 200.2 MB (200196508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c71033fb9b69c2dacee54e49fdc25f819d83bc48f3048605a84f425e9e2c212`  
		Last Modified: Sun, 29 May 2022 05:36:20 GMT  
		Size: 292.0 MB (291965870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaf7412f3f13859bf1fc4a345cf78780035b159f835195638be0005ecd61395`  
		Last Modified: Sun, 29 May 2022 05:36:01 GMT  
		Size: 2.4 MB (2381173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185d6e2c4e06c1f88129c732367b5129c2bac51473df263e1e288e73f6067edf`  
		Last Modified: Sun, 29 May 2022 05:36:01 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255dd54377156de8cc8dcd32e92b7c1e1cf8870a9c2e9a67d3b41098c860a184`  
		Last Modified: Sun, 29 May 2022 05:36:01 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4ab1dc98c79e1be194d7ee0d966751e54dda2dfdaed1ef45e115f344c64ee`  
		Last Modified: Sun, 29 May 2022 05:36:01 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe59db26306e044dca8b6cfb022029178fc471a01ca4fb88013b6255803fdbd`  
		Last Modified: Sun, 29 May 2022 05:36:01 GMT  
		Size: 2.5 KB (2499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:d4913450f9eb5e2aba74d4506148b03e8140bf917a16a29ed0f1371316bb9a5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **623.4 MB (623421560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec22746512ae9867b37ca7566f9d3c224272b6dd6c34271219551ef4c8293dce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Sat, 28 May 2022 00:40:23 GMT
ADD file:a78273677555ebe8bac187f491203093eec62fa1c4f65f00ba2cf0cc2230992f in / 
# Sat, 28 May 2022 00:40:24 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:05:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 16:50:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:50:24 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 28 May 2022 16:50:25 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Sat, 28 May 2022 16:50:26 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 16:50:27 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 16:50:28 GMT
ENV JAVA_VERSION=11.0.15
# Sat, 28 May 2022 16:50:36 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_11.0.15_10.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_11.0.15_10.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Sat, 28 May 2022 20:03:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 28 May 2022 20:03:46 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 20:03:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 28 May 2022 20:03:48 GMT
WORKDIR /usr/local/tomcat
# Sat, 28 May 2022 20:03:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 28 May 2022 20:03:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 28 May 2022 20:19:40 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 28 May 2022 20:19:41 GMT
ENV TOMCAT_MAJOR=9
# Sat, 28 May 2022 20:19:42 GMT
ENV TOMCAT_VERSION=9.0.63
# Sat, 28 May 2022 20:19:43 GMT
ENV TOMCAT_SHA512=4b905018164026756bd36ab9fde8f6b21c886acb8e5255d93f8938491e4d375dd18b9fc58ee23e3d78b16e8b81271c1c998e5592beedcac632567c2ca9411c69
# Sat, 28 May 2022 20:19:45 GMT
COPY dir:89b6eab438e77990f83a7f8db9b9f099a2b07725410586e3046894ac9c43563e in /usr/local/tomcat 
# Sat, 28 May 2022 20:19:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:19:50 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 28 May 2022 20:19:51 GMT
EXPOSE 8080
# Sat, 28 May 2022 20:19:52 GMT
CMD ["catalina.sh" "run"]
# Sun, 29 May 2022 07:52:39 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sun, 29 May 2022 07:52:39 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sun, 29 May 2022 07:52:40 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sun, 29 May 2022 07:52:41 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sun, 29 May 2022 07:52:42 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sun, 29 May 2022 07:52:43 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sun, 29 May 2022 07:53:30 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:53:31 GMT
ENV XWIKI_VERSION=14.4
# Sun, 29 May 2022 07:53:32 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.4
# Sun, 29 May 2022 07:53:33 GMT
ENV XWIKI_DOWNLOAD_SHA256=313983ea4e1c8f7f44058bedf150e61b9b57a0a9c00c99b3a6471a4f567010e3
# Sun, 29 May 2022 07:54:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sun, 29 May 2022 07:54:48 GMT
ENV MYSQL_JDBC_VERSION=8.0.29
# Sun, 29 May 2022 07:54:49 GMT
ENV MYSQL_JDBC_SHA256=d4e32d2a6026b5acc00300b73a86c28fb92681ae9629b21048ee67014c911db6
# Sun, 29 May 2022 07:54:50 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.29
# Sun, 29 May 2022 07:54:51 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.29.jar
# Sun, 29 May 2022 07:54:52 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.29.jar
# Sun, 29 May 2022 07:54:53 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sun, 29 May 2022 07:54:55 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sun, 29 May 2022 07:54:56 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sun, 29 May 2022 07:54:57 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sun, 29 May 2022 07:54:58 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sun, 29 May 2022 07:54:59 GMT
VOLUME [/usr/local/xwiki]
# Sun, 29 May 2022 07:55:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 07:55:00 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:d794814721d57f8aaec06ab3652e90212cc3beccf5ff5c87f6ecf8375784bcc8`  
		Last Modified: Sat, 28 May 2022 00:47:04 GMT  
		Size: 53.7 MB (53696947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf62ee63325dbbad699d6845f68c2391db3bf158f60373849c2d1cb6bb479788`  
		Last Modified: Sat, 28 May 2022 11:17:05 GMT  
		Size: 4.9 MB (4938744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e37b4c58dd1db7ead6f3c2cdf757f490b4e29c958d2a70559c313e9a03a5ef`  
		Last Modified: Sat, 28 May 2022 11:17:06 GMT  
		Size: 10.7 MB (10657073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29312e2f0b2d2423a19b1e65da0020d22da272698007d994eb022cafc68c98dc`  
		Last Modified: Sat, 28 May 2022 17:06:29 GMT  
		Size: 5.6 MB (5649779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd89bea478de23120f9e854c805b853218e7d1c2b55ab2f0d9fa8a312c41bf12`  
		Last Modified: Sat, 28 May 2022 17:06:29 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28ea084fee99e1a8783492e9519624f9d393b283f712e81f1af19c68ce1ce2a`  
		Last Modified: Sat, 28 May 2022 17:06:36 GMT  
		Size: 46.5 MB (46498872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0d4a73df71717612d4f66dd4836687d3d09cf2d630603fdd04ec76af94b297`  
		Last Modified: Sat, 28 May 2022 20:53:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6598f168c59e37880ea4a9683e9e7c3211488dbeaec2a19a813e870f7f6a9c7`  
		Last Modified: Sat, 28 May 2022 21:06:11 GMT  
		Size: 12.2 MB (12162557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20dce81c566bea5107a898bb605d7362d64a509efae89cd502dd4ecfb1c4ede`  
		Last Modified: Sat, 28 May 2022 21:06:10 GMT  
		Size: 217.2 KB (217167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d792bc67d379de4c694c7ef218e9c15c070cde2ff9f2eb493970ab8277470f3c`  
		Last Modified: Sun, 29 May 2022 08:01:12 GMT  
		Size: 195.2 MB (195240942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba53e888b3bc77a8ec9319eab754dfbe13882b5fd21adeed86508732672e83c`  
		Last Modified: Sun, 29 May 2022 08:01:07 GMT  
		Size: 292.0 MB (291965970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f70e936b223f6e34c2dd5d599878ee6ed8903fa2e8890bfc2af1a74dae34cd`  
		Last Modified: Sun, 29 May 2022 08:00:45 GMT  
		Size: 2.4 MB (2381165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf4bc49f651c92a159a7d8de3a0d51d13a595e7fa55a8f623b4316c75bcfc18`  
		Last Modified: Sun, 29 May 2022 08:00:45 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b7a06e8a7bb8bdebf40eb83f828b5c794381a7af40ad5cdcd98ea0dea3dc8`  
		Last Modified: Sun, 29 May 2022 08:00:45 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074f3a16435cae6d2aea709530e7566379212596597c1c5ff4828536a51b900e`  
		Last Modified: Sun, 29 May 2022 08:00:45 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e18a0f64b3094efd1cc12e29d2668e8d775002f17b4fd19511ce5df54ce1418`  
		Last Modified: Sun, 29 May 2022 08:00:45 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
