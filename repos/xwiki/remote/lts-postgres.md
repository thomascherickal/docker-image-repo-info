## `xwiki:lts-postgres`

```console
$ docker pull xwiki@sha256:f42594768a623a30a23391828b852e9889eb71b5a4b11c3fd8322a2b3e6c9055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:a61cd40fb4c0b0cb77e004e778782218338b2cb7837716b840d1e5a6bfaa66bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **631.0 MB (631049623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05b87ee458cbdfa5bdb8bf5ded6706861a88d35dc550fc1c34cadce0c450efc`
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
# Sun, 29 May 2022 05:32:44 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 05:34:26 GMT
ENV XWIKI_VERSION=13.10.6
# Sun, 29 May 2022 05:34:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.6
# Sun, 29 May 2022 05:34:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=0ffeef24fc49a78a66e4204514f3b258af739be70840291797f99879a8d1d4fe
# Sun, 29 May 2022 05:35:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sun, 29 May 2022 05:35:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sun, 29 May 2022 05:35:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sun, 29 May 2022 05:35:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sun, 29 May 2022 05:35:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sun, 29 May 2022 05:35:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sun, 29 May 2022 05:35:06 GMT
VOLUME [/usr/local/xwiki]
# Sun, 29 May 2022 05:35:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 05:35:06 GMT
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
	-	`sha256:26704cc23b6b6b9bf159bf3766baa8a7442c91bf0c762257591eb4944083684e`  
		Last Modified: Sun, 29 May 2022 05:37:41 GMT  
		Size: 201.1 MB (201062749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2140059fee02a61ec41a319d94886382b732581f0359b7ec74933a440a276c`  
		Last Modified: Sun, 29 May 2022 05:39:39 GMT  
		Size: 292.6 MB (292623809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617b69b0ec46755fdc387f5748cb35d82f80d027634762310f71a0250bf8e0bf`  
		Last Modified: Sun, 29 May 2022 05:39:22 GMT  
		Size: 846.2 KB (846202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904d8a809239c2a7349d43f08b18a4b103bda4b408f42ee94836d5416e19a89c`  
		Last Modified: Sun, 29 May 2022 05:39:21 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c768f2e1d07e26f971fcc1ed2669b7e9bcba17780088945827e7b11bae33c27`  
		Last Modified: Sun, 29 May 2022 05:39:22 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2b0c6e077c0bfe10ac30c6b043166d98cb7ef475dae6337c49d69d4d8db795`  
		Last Modified: Sun, 29 May 2022 05:39:21 GMT  
		Size: 5.3 KB (5331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6dcd88385263c7935f406552b7cf07a151c7c5ba1fa0eb8debea7450ccca75`  
		Last Modified: Sun, 29 May 2022 05:39:21 GMT  
		Size: 2.5 KB (2501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:a4bf4da7bf4ea5c24613c3c30ac9dad717ddbb92322edb1af17115a155129345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **623.4 MB (623397927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef1eb0d900a80a1bd14b5791ee2e51f7e540a4270f8fa1f6c52d6eb24d60020`
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
# Sun, 29 May 2022 07:55:49 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:57:53 GMT
ENV XWIKI_VERSION=13.10.6
# Sun, 29 May 2022 07:57:53 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.6
# Sun, 29 May 2022 07:57:54 GMT
ENV XWIKI_DOWNLOAD_SHA256=0ffeef24fc49a78a66e4204514f3b258af739be70840291797f99879a8d1d4fe
# Sun, 29 May 2022 07:58:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sun, 29 May 2022 07:58:45 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sun, 29 May 2022 07:58:46 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sun, 29 May 2022 07:58:47 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sun, 29 May 2022 07:58:48 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sun, 29 May 2022 07:58:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sun, 29 May 2022 07:58:50 GMT
VOLUME [/usr/local/xwiki]
# Sun, 29 May 2022 07:58:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 07:58:52 GMT
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
	-	`sha256:04e80386afb77022e05deeaf1b3e3c72892cc20a9578020d014530b21e1aa1d4`  
		Last Modified: Sun, 29 May 2022 08:02:27 GMT  
		Size: 196.1 MB (196094569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1340ac10cfda28d6506fca00515cda7325570c510ca6908736ef44c47e759`  
		Last Modified: Sun, 29 May 2022 08:04:46 GMT  
		Size: 292.6 MB (292624041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62895406e31126ec341b5d024668b004e815ad91d295be36a6b5f6129df32db`  
		Last Modified: Sun, 29 May 2022 08:04:24 GMT  
		Size: 846.2 KB (846203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4728dd0e0455eddff1699988d07d191673ce9c81ecf805dc9fe36e666a6640`  
		Last Modified: Sun, 29 May 2022 08:04:24 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56691fb9d1f4dd281d209640281d8770c7c5c9c710f06ce845beb1e9412f0fde`  
		Last Modified: Sun, 29 May 2022 08:04:24 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a901c6e0610a827372fdf5d38ef06b9f076f0224c9dd377c54bd1b556e471b8b`  
		Last Modified: Sun, 29 May 2022 08:04:24 GMT  
		Size: 5.3 KB (5331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5da170b85dbcb45fb567f807079047547f86ac99ec9ceaea7358de1fa535007`  
		Last Modified: Sun, 29 May 2022 08:04:24 GMT  
		Size: 2.5 KB (2503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
