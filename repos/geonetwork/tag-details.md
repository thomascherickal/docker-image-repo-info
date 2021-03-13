<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `geonetwork`

-	[`geonetwork:3`](#geonetwork3)
-	[`geonetwork:3-postgres`](#geonetwork3-postgres)
-	[`geonetwork:3.10`](#geonetwork310)
-	[`geonetwork:3.10-postgres`](#geonetwork310-postgres)
-	[`geonetwork:3.10.6`](#geonetwork3106)
-	[`geonetwork:3.10.6-postgres`](#geonetwork3106-postgres)
-	[`geonetwork:3.8`](#geonetwork38)
-	[`geonetwork:3.8-postgres`](#geonetwork38-postgres)
-	[`geonetwork:3.8.3`](#geonetwork383)
-	[`geonetwork:3.8.3-postgres`](#geonetwork383-postgres)
-	[`geonetwork:4`](#geonetwork4)
-	[`geonetwork:4.0`](#geonetwork40)
-	[`geonetwork:4.0.2`](#geonetwork402)
-	[`geonetwork:latest`](#geonetworklatest)
-	[`geonetwork:postgres`](#geonetworkpostgres)

## `geonetwork:3`

```console
$ docker pull geonetwork@sha256:8005e3f452063d780e75dd3b6613f0fd438c3d8b1cfed512b0a7f92a970e3695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3` - linux; amd64

```console
$ docker pull geonetwork@sha256:fb1f17d336069ea2da9d72e1874ea432c710410d7e8360645b995cedb776216b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **519.1 MB (519102348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a25cd8b79a18b9482efc42acfdd8be05fc271ce2fab2704724c675fdb3558e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3-postgres`

```console
$ docker pull geonetwork@sha256:4b830af6894c21a1b32caf0f6b3ae8c312ae080b434212dfb4c97289ab0e8875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:2c493caa78291f25a68bf9aa990c521d1e221bcd9408386fdce27d3b7d5d7a38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530916900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99897c81763086863923bef414936150d272b7b4e2952e9f8716ca810142b492`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:43 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:49:45 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c920f73da2989271e2382be78f711f9fe387c9269b86fce1e61a19207afe330`  
		Last Modified: Sat, 13 Mar 2021 17:53:12 GMT  
		Size: 11.8 MB (11811193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8687146be4475b3d4c07af558b42490c128f1cd82948bac69f1ec29d419480`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b7a8a7be8baae902523b3780415e419cb6b79bdbb67ceea8d5995bb86eca56`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87026b8b7e2b9b076dd17821dc017776fe8030776141233077f19b821ba15e1`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10`

```console
$ docker pull geonetwork@sha256:8005e3f452063d780e75dd3b6613f0fd438c3d8b1cfed512b0a7f92a970e3695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.10` - linux; amd64

```console
$ docker pull geonetwork@sha256:fb1f17d336069ea2da9d72e1874ea432c710410d7e8360645b995cedb776216b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **519.1 MB (519102348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a25cd8b79a18b9482efc42acfdd8be05fc271ce2fab2704724c675fdb3558e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10-postgres`

```console
$ docker pull geonetwork@sha256:4b830af6894c21a1b32caf0f6b3ae8c312ae080b434212dfb4c97289ab0e8875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.10-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:2c493caa78291f25a68bf9aa990c521d1e221bcd9408386fdce27d3b7d5d7a38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530916900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99897c81763086863923bef414936150d272b7b4e2952e9f8716ca810142b492`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:43 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:49:45 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c920f73da2989271e2382be78f711f9fe387c9269b86fce1e61a19207afe330`  
		Last Modified: Sat, 13 Mar 2021 17:53:12 GMT  
		Size: 11.8 MB (11811193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8687146be4475b3d4c07af558b42490c128f1cd82948bac69f1ec29d419480`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b7a8a7be8baae902523b3780415e419cb6b79bdbb67ceea8d5995bb86eca56`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87026b8b7e2b9b076dd17821dc017776fe8030776141233077f19b821ba15e1`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10.6`

```console
$ docker pull geonetwork@sha256:8005e3f452063d780e75dd3b6613f0fd438c3d8b1cfed512b0a7f92a970e3695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.10.6` - linux; amd64

```console
$ docker pull geonetwork@sha256:fb1f17d336069ea2da9d72e1874ea432c710410d7e8360645b995cedb776216b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **519.1 MB (519102348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a25cd8b79a18b9482efc42acfdd8be05fc271ce2fab2704724c675fdb3558e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10.6-postgres`

```console
$ docker pull geonetwork@sha256:4b830af6894c21a1b32caf0f6b3ae8c312ae080b434212dfb4c97289ab0e8875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.10.6-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:2c493caa78291f25a68bf9aa990c521d1e221bcd9408386fdce27d3b7d5d7a38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530916900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99897c81763086863923bef414936150d272b7b4e2952e9f8716ca810142b492`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:43 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:49:45 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c920f73da2989271e2382be78f711f9fe387c9269b86fce1e61a19207afe330`  
		Last Modified: Sat, 13 Mar 2021 17:53:12 GMT  
		Size: 11.8 MB (11811193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8687146be4475b3d4c07af558b42490c128f1cd82948bac69f1ec29d419480`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b7a8a7be8baae902523b3780415e419cb6b79bdbb67ceea8d5995bb86eca56`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87026b8b7e2b9b076dd17821dc017776fe8030776141233077f19b821ba15e1`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.8`

```console
$ docker pull geonetwork@sha256:46c2220ab2e0728743a371712d5ca3e2747fc5848b47e359591e9217fd451c20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.8` - linux; amd64

```console
$ docker pull geonetwork@sha256:ebf0a8b35db54613c2b44e91261aa924e4243beddcaff92fb069b338bb36ff6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448548121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e2b19a0073f0af4d6188c7247697f6e0adc8982dacad875a0808de1b1aeb05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_VERSION=3.8.3
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_DOWNLOAD_MD5=0d05c65aa4ac67fea90fa74f947822d6
# Sat, 13 Mar 2021 17:49:49 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:50:11 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/geonetwork.war/download &&      echo "$GN_DOWNLOAD_MD5 *$GN_FILE" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:50:12 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fde1b37248a74df0b84507397d40b1eb71dc76195c49f0eef3646f71354e9b`  
		Last Modified: Sat, 13 Mar 2021 17:53:44 GMT  
		Size: 205.7 MB (205747889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44609d004582a89752a4cd3943a24518dba9bac08beda57ae7fe9dca897c0ca6`  
		Last Modified: Sat, 13 Mar 2021 17:53:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.8-postgres`

```console
$ docker pull geonetwork@sha256:5bc3d959577ad3b95bb1ab90766ccb2470af660039421c6eb81d232e1b496d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.8-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:e37c4c5442466b1519618c5a27a2a7ad23dbc63f476e877ee6802c13851cda6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.4 MB (460362196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa43f29a0a63cafaa77c06c058c2050336d1ca182f2181b2c8eb6c7d697aa16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_VERSION=3.8.3
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_DOWNLOAD_MD5=0d05c65aa4ac67fea90fa74f947822d6
# Sat, 13 Mar 2021 17:49:49 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:50:11 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/geonetwork.war/download &&      echo "$GN_DOWNLOAD_MD5 *$GN_FILE" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:50:12 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:12 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:50:27 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:50:28 GMT
RUN sed -i -e 's#<import resource="../config-db/h2.xml"/>#<!--<import resource="../config-db/h2.xml"/> -->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:50:28 GMT
COPY file:2dedfd940a86106b2ae284c537f14d365881c03a01b212f81b49177bb22c8d7a in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:50:28 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fde1b37248a74df0b84507397d40b1eb71dc76195c49f0eef3646f71354e9b`  
		Last Modified: Sat, 13 Mar 2021 17:53:44 GMT  
		Size: 205.7 MB (205747889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44609d004582a89752a4cd3943a24518dba9bac08beda57ae7fe9dca897c0ca6`  
		Last Modified: Sat, 13 Mar 2021 17:53:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bae0e2cb2af185ac9f3f195f48c68f9b558ef1e2b218f696d51460f41817f71`  
		Last Modified: Sat, 13 Mar 2021 17:53:58 GMT  
		Size: 11.8 MB (11811291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf04f799c4bf9edcb44d56e93ae217c6fca8dc70ec477e95770f2b5b024f257a`  
		Last Modified: Sat, 13 Mar 2021 17:53:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac95018806924c2b855f11a4ea5c9c68298aaa0c79262b8514d38ff412c379e`  
		Last Modified: Sat, 13 Mar 2021 17:53:55 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0e19ad3ca7db583985caec311d48cfa4a23cdbf6b3cdbe8d985113a97f873`  
		Last Modified: Sat, 13 Mar 2021 17:53:56 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.8.3`

```console
$ docker pull geonetwork@sha256:46c2220ab2e0728743a371712d5ca3e2747fc5848b47e359591e9217fd451c20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.8.3` - linux; amd64

```console
$ docker pull geonetwork@sha256:ebf0a8b35db54613c2b44e91261aa924e4243beddcaff92fb069b338bb36ff6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.5 MB (448548121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e2b19a0073f0af4d6188c7247697f6e0adc8982dacad875a0808de1b1aeb05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_VERSION=3.8.3
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_DOWNLOAD_MD5=0d05c65aa4ac67fea90fa74f947822d6
# Sat, 13 Mar 2021 17:49:49 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:50:11 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/geonetwork.war/download &&      echo "$GN_DOWNLOAD_MD5 *$GN_FILE" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:50:12 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fde1b37248a74df0b84507397d40b1eb71dc76195c49f0eef3646f71354e9b`  
		Last Modified: Sat, 13 Mar 2021 17:53:44 GMT  
		Size: 205.7 MB (205747889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44609d004582a89752a4cd3943a24518dba9bac08beda57ae7fe9dca897c0ca6`  
		Last Modified: Sat, 13 Mar 2021 17:53:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.8.3-postgres`

```console
$ docker pull geonetwork@sha256:5bc3d959577ad3b95bb1ab90766ccb2470af660039421c6eb81d232e1b496d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:3.8.3-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:e37c4c5442466b1519618c5a27a2a7ad23dbc63f476e877ee6802c13851cda6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.4 MB (460362196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa43f29a0a63cafaa77c06c058c2050336d1ca182f2181b2c8eb6c7d697aa16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_VERSION=3.8.3
# Sat, 13 Mar 2021 17:49:49 GMT
ENV GN_DOWNLOAD_MD5=0d05c65aa4ac67fea90fa74f947822d6
# Sat, 13 Mar 2021 17:49:49 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:50:11 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/geonetwork.war/download &&      echo "$GN_DOWNLOAD_MD5 *$GN_FILE" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:50:12 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:12 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:50:27 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:50:28 GMT
RUN sed -i -e 's#<import resource="../config-db/h2.xml"/>#<!--<import resource="../config-db/h2.xml"/> -->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:50:28 GMT
COPY file:2dedfd940a86106b2ae284c537f14d365881c03a01b212f81b49177bb22c8d7a in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:50:28 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:50:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:50:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fde1b37248a74df0b84507397d40b1eb71dc76195c49f0eef3646f71354e9b`  
		Last Modified: Sat, 13 Mar 2021 17:53:44 GMT  
		Size: 205.7 MB (205747889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44609d004582a89752a4cd3943a24518dba9bac08beda57ae7fe9dca897c0ca6`  
		Last Modified: Sat, 13 Mar 2021 17:53:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bae0e2cb2af185ac9f3f195f48c68f9b558ef1e2b218f696d51460f41817f71`  
		Last Modified: Sat, 13 Mar 2021 17:53:58 GMT  
		Size: 11.8 MB (11811291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf04f799c4bf9edcb44d56e93ae217c6fca8dc70ec477e95770f2b5b024f257a`  
		Last Modified: Sat, 13 Mar 2021 17:53:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac95018806924c2b855f11a4ea5c9c68298aaa0c79262b8514d38ff412c379e`  
		Last Modified: Sat, 13 Mar 2021 17:53:55 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d0e19ad3ca7db583985caec311d48cfa4a23cdbf6b3cdbe8d985113a97f873`  
		Last Modified: Sat, 13 Mar 2021 17:53:56 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4`

```console
$ docker pull geonetwork@sha256:3aedb60b99aed96a608bd2f669e59c3ec850943f1fc248970693bf97b5f7e80e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:4` - linux; amd64

```console
$ docker pull geonetwork@sha256:02a8c9eb86c85eef39bfc5da7cb94c95c440503776edd86a617a4684172ecff9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.1 MB (426119385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e9cde182c1a018ea6b3017b8dc47b7bc815373c3b9796a20c7708163c807a5`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 22:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:16:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:16:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:16:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:16:35 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:16:35 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:16:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_VERSION=9.4.38.v20210224
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.38.v20210224/jetty-home-9.4.38.v20210224.tar.gz
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Sat, 13 Mar 2021 12:54:51 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			p80.pool.sks-keyservers.net:80 			ipv4.pool.sks-keyservers.net 			pgp.mit.edu ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 13 Mar 2021 12:54:51 GMT
WORKDIR /var/lib/jetty
# Sat, 13 Mar 2021 12:54:51 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Sat, 13 Mar 2021 12:54:51 GMT
USER jetty
# Sat, 13 Mar 2021 12:54:52 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 12:54:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 12:54:52 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:50:32 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 13 Mar 2021 17:50:33 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 13 Mar 2021 17:50:33 GMT
USER root
# Sat, 13 Mar 2021 17:50:37 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 13 Mar 2021 17:50:37 GMT
USER jetty
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_FILE=GeoNetwork-4.0.2-0.war
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_VERSION=4.0.2
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_DOWNLOAD_MD5=3009549f23b6aca6ebdd851c5bf512b8
# Sat, 13 Mar 2021 17:52:08 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&     curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 13 Mar 2021 17:52:09 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Sat, 13 Mar 2021 17:52:09 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 13 Mar 2021 17:52:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:52:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6c60bfcb211ff0f5957d57dfa2de90348eae270690abdd725353594266d802`  
		Last Modified: Fri, 12 Mar 2021 22:28:51 GMT  
		Size: 5.5 MB (5531061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ee52e88d8b51becf74134f07ed6950cb58555ebd9e0774bd9bc524ea3c5f09`  
		Last Modified: Fri, 12 Mar 2021 22:31:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd26b251c915a3c1192d6be0d04c5be894bb0a22c45640f888ccdc6f7029a38`  
		Last Modified: Fri, 12 Mar 2021 22:31:08 GMT  
		Size: 41.3 MB (41319832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28de71d5998158b296dc4a49b532ae8f8085aa31070003f8c741e66ee7eda17`  
		Last Modified: Sat, 13 Mar 2021 12:59:39 GMT  
		Size: 9.8 MB (9821644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188030475068766a69993fe0002bd0bcb58a2f3d9a5ccad0aff86f6fb89120f1`  
		Last Modified: Sat, 13 Mar 2021 12:59:38 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b897acc17e64685871079597edf79fe56c889e5ad9542528c696ecbc088e9fe6`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f612801b36ac9f8203331d83fa22c84d55a6f1708b827fe09a0ef03a7ba975`  
		Last Modified: Sat, 13 Mar 2021 17:54:32 GMT  
		Size: 301.2 MB (301213742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d480b2892b856d7ef2bec0d98323b015ff4a6b02352999b0a6aae84fc6c4b71`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.0`

```console
$ docker pull geonetwork@sha256:3aedb60b99aed96a608bd2f669e59c3ec850943f1fc248970693bf97b5f7e80e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:4.0` - linux; amd64

```console
$ docker pull geonetwork@sha256:02a8c9eb86c85eef39bfc5da7cb94c95c440503776edd86a617a4684172ecff9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.1 MB (426119385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e9cde182c1a018ea6b3017b8dc47b7bc815373c3b9796a20c7708163c807a5`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 22:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:16:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:16:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:16:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:16:35 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:16:35 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:16:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_VERSION=9.4.38.v20210224
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.38.v20210224/jetty-home-9.4.38.v20210224.tar.gz
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Sat, 13 Mar 2021 12:54:51 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			p80.pool.sks-keyservers.net:80 			ipv4.pool.sks-keyservers.net 			pgp.mit.edu ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 13 Mar 2021 12:54:51 GMT
WORKDIR /var/lib/jetty
# Sat, 13 Mar 2021 12:54:51 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Sat, 13 Mar 2021 12:54:51 GMT
USER jetty
# Sat, 13 Mar 2021 12:54:52 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 12:54:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 12:54:52 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:50:32 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 13 Mar 2021 17:50:33 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 13 Mar 2021 17:50:33 GMT
USER root
# Sat, 13 Mar 2021 17:50:37 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 13 Mar 2021 17:50:37 GMT
USER jetty
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_FILE=GeoNetwork-4.0.2-0.war
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_VERSION=4.0.2
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_DOWNLOAD_MD5=3009549f23b6aca6ebdd851c5bf512b8
# Sat, 13 Mar 2021 17:52:08 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&     curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 13 Mar 2021 17:52:09 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Sat, 13 Mar 2021 17:52:09 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 13 Mar 2021 17:52:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:52:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6c60bfcb211ff0f5957d57dfa2de90348eae270690abdd725353594266d802`  
		Last Modified: Fri, 12 Mar 2021 22:28:51 GMT  
		Size: 5.5 MB (5531061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ee52e88d8b51becf74134f07ed6950cb58555ebd9e0774bd9bc524ea3c5f09`  
		Last Modified: Fri, 12 Mar 2021 22:31:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd26b251c915a3c1192d6be0d04c5be894bb0a22c45640f888ccdc6f7029a38`  
		Last Modified: Fri, 12 Mar 2021 22:31:08 GMT  
		Size: 41.3 MB (41319832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28de71d5998158b296dc4a49b532ae8f8085aa31070003f8c741e66ee7eda17`  
		Last Modified: Sat, 13 Mar 2021 12:59:39 GMT  
		Size: 9.8 MB (9821644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188030475068766a69993fe0002bd0bcb58a2f3d9a5ccad0aff86f6fb89120f1`  
		Last Modified: Sat, 13 Mar 2021 12:59:38 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b897acc17e64685871079597edf79fe56c889e5ad9542528c696ecbc088e9fe6`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f612801b36ac9f8203331d83fa22c84d55a6f1708b827fe09a0ef03a7ba975`  
		Last Modified: Sat, 13 Mar 2021 17:54:32 GMT  
		Size: 301.2 MB (301213742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d480b2892b856d7ef2bec0d98323b015ff4a6b02352999b0a6aae84fc6c4b71`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.0.2`

```console
$ docker pull geonetwork@sha256:3aedb60b99aed96a608bd2f669e59c3ec850943f1fc248970693bf97b5f7e80e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:4.0.2` - linux; amd64

```console
$ docker pull geonetwork@sha256:02a8c9eb86c85eef39bfc5da7cb94c95c440503776edd86a617a4684172ecff9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.1 MB (426119385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e9cde182c1a018ea6b3017b8dc47b7bc815373c3b9796a20c7708163c807a5`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 22:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:16:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:16:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:16:34 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:16:35 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:16:35 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:16:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_VERSION=9.4.38.v20210224
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 13 Mar 2021 12:54:46 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 13 Mar 2021 12:54:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.38.v20210224/jetty-home-9.4.38.v20210224.tar.gz
# Sat, 13 Mar 2021 12:54:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Sat, 13 Mar 2021 12:54:51 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			p80.pool.sks-keyservers.net:80 			ipv4.pool.sks-keyservers.net 			pgp.mit.edu ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 13 Mar 2021 12:54:51 GMT
WORKDIR /var/lib/jetty
# Sat, 13 Mar 2021 12:54:51 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Sat, 13 Mar 2021 12:54:51 GMT
USER jetty
# Sat, 13 Mar 2021 12:54:52 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 12:54:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Mar 2021 12:54:52 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:50:32 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 13 Mar 2021 17:50:33 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 13 Mar 2021 17:50:33 GMT
USER root
# Sat, 13 Mar 2021 17:50:37 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 13 Mar 2021 17:50:37 GMT
USER jetty
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_FILE=GeoNetwork-4.0.2-0.war
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_VERSION=4.0.2
# Sat, 13 Mar 2021 17:50:37 GMT
ENV GN_DOWNLOAD_MD5=3009549f23b6aca6ebdd851c5bf512b8
# Sat, 13 Mar 2021 17:52:08 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&     curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 13 Mar 2021 17:52:09 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Sat, 13 Mar 2021 17:52:09 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 13 Mar 2021 17:52:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 13 Mar 2021 17:52:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6c60bfcb211ff0f5957d57dfa2de90348eae270690abdd725353594266d802`  
		Last Modified: Fri, 12 Mar 2021 22:28:51 GMT  
		Size: 5.5 MB (5531061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ee52e88d8b51becf74134f07ed6950cb58555ebd9e0774bd9bc524ea3c5f09`  
		Last Modified: Fri, 12 Mar 2021 22:31:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd26b251c915a3c1192d6be0d04c5be894bb0a22c45640f888ccdc6f7029a38`  
		Last Modified: Fri, 12 Mar 2021 22:31:08 GMT  
		Size: 41.3 MB (41319832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28de71d5998158b296dc4a49b532ae8f8085aa31070003f8c741e66ee7eda17`  
		Last Modified: Sat, 13 Mar 2021 12:59:39 GMT  
		Size: 9.8 MB (9821644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188030475068766a69993fe0002bd0bcb58a2f3d9a5ccad0aff86f6fb89120f1`  
		Last Modified: Sat, 13 Mar 2021 12:59:38 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b897acc17e64685871079597edf79fe56c889e5ad9542528c696ecbc088e9fe6`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f612801b36ac9f8203331d83fa22c84d55a6f1708b827fe09a0ef03a7ba975`  
		Last Modified: Sat, 13 Mar 2021 17:54:32 GMT  
		Size: 301.2 MB (301213742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d480b2892b856d7ef2bec0d98323b015ff4a6b02352999b0a6aae84fc6c4b71`  
		Last Modified: Sat, 13 Mar 2021 17:54:09 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:latest`

```console
$ docker pull geonetwork@sha256:8005e3f452063d780e75dd3b6613f0fd438c3d8b1cfed512b0a7f92a970e3695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:latest` - linux; amd64

```console
$ docker pull geonetwork@sha256:fb1f17d336069ea2da9d72e1874ea432c710410d7e8360645b995cedb776216b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **519.1 MB (519102348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a25cd8b79a18b9482efc42acfdd8be05fc271ce2fab2704724c675fdb3558e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:postgres`

```console
$ docker pull geonetwork@sha256:4b830af6894c21a1b32caf0f6b3ae8c312ae080b434212dfb4c97289ab0e8875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `geonetwork:postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:2c493caa78291f25a68bf9aa990c521d1e221bcd9408386fdce27d3b7d5d7a38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530916900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99897c81763086863923bef414936150d272b7b4e2952e9f8716ca810142b492`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 22:15:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 12 Mar 2021 22:15:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 22:15:46 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 22:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 22:15:47 GMT
ENV JAVA_VERSION=8u282
# Fri, 12 Mar 2021 22:15:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 13 Mar 2021 15:26:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 13 Mar 2021 15:26:48 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Mar 2021 15:26:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 13 Mar 2021 15:26:49 GMT
WORKDIR /usr/local/tomcat
# Sat, 13 Mar 2021 15:26:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:26:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 13 Mar 2021 15:35:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_MAJOR=8
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_VERSION=8.5.64
# Sat, 13 Mar 2021 15:35:12 GMT
ENV TOMCAT_SHA512=4b63a55b7beb38a3be6cbaeec525a596c8aeddfd595bd0c6d23f282af709085fcc4f526e3a577c58201d93b71c0f4d3a1a4abf8c2f886c4f7911d8dcfb839280
# Sat, 13 Mar 2021 15:35:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 13 Mar 2021 15:35:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 13 Mar 2021 15:35:40 GMT
EXPOSE 8080
# Sat, 13 Mar 2021 15:35:40 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_FILE=geonetwork.war
# Sat, 13 Mar 2021 17:49:00 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 13 Mar 2021 17:49:00 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_VERSION=3.10.6
# Sat, 13 Mar 2021 17:49:00 GMT
ENV GN_DOWNLOAD_MD5=6f6980788a4df8477b20aa114bae2ef9
# Sat, 13 Mar 2021 17:49:01 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 13 Mar 2021 17:49:29 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 13 Mar 2021 17:49:30 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:31 GMT
CMD ["catalina.sh" "run"]
# Sat, 13 Mar 2021 17:49:43 GMT
RUN apt-get update && apt-get install -y postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 17:49:45 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' $CATALINA_HOME/webapps/geonetwork/WEB-INF/config-node/srv.xml
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 13 Mar 2021 17:49:45 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 13 Mar 2021 17:49:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 13 Mar 2021 17:49:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c39da3e61dffe0979f3c7318d6e709032d75cf51066b3b707772d9ddbe8753`  
		Last Modified: Fri, 12 Mar 2021 22:27:03 GMT  
		Size: 5.3 MB (5286487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c6215cb41b9e3de83884c7ae653bd6acf03d9475cd7814318f35e6407c2c0a`  
		Last Modified: Fri, 12 Mar 2021 22:29:52 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a77a74e1e1406c4c0521505675193d0922b664719c97595bf65973270f50c8`  
		Last Modified: Fri, 12 Mar 2021 22:30:05 GMT  
		Size: 105.9 MB (105913875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eae4b1a3aa7dbd9076e54b5461c8e731291715b0bb6d46c3b77ea4a27ed68ed`  
		Last Modified: Sat, 13 Mar 2021 15:43:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa649503be0f10cbd3155eefa7cdb2621e2ec4d9fe631320e089e3ad2640c84d`  
		Last Modified: Sat, 13 Mar 2021 15:50:45 GMT  
		Size: 11.5 MB (11529629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c3b4aa26636cbed501774f2e75e4f251f3550c27244051b5337566d1eca04`  
		Last Modified: Sat, 13 Mar 2021 15:50:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1451a7cba092737a797a1530bcb6d85ea0552f79a74f522b8cb8613b102ccf28`  
		Last Modified: Sat, 13 Mar 2021 17:52:51 GMT  
		Size: 276.3 MB (276302115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7579f1de02314767f3bbd1102517b23bc3b076565745b987e99f3a93304285f`  
		Last Modified: Sat, 13 Mar 2021 17:52:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c920f73da2989271e2382be78f711f9fe387c9269b86fce1e61a19207afe330`  
		Last Modified: Sat, 13 Mar 2021 17:53:12 GMT  
		Size: 11.8 MB (11811193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8687146be4475b3d4c07af558b42490c128f1cd82948bac69f1ec29d419480`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b7a8a7be8baae902523b3780415e419cb6b79bdbb67ceea8d5995bb86eca56`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87026b8b7e2b9b076dd17821dc017776fe8030776141233077f19b821ba15e1`  
		Last Modified: Sat, 13 Mar 2021 17:53:10 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
