<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `geonetwork`

-	[`geonetwork:3`](#geonetwork3)
-	[`geonetwork:3-postgres`](#geonetwork3-postgres)
-	[`geonetwork:3.10`](#geonetwork310)
-	[`geonetwork:3.10-postgres`](#geonetwork310-postgres)
-	[`geonetwork:3.10.10`](#geonetwork31010)
-	[`geonetwork:3.10.10-postgres`](#geonetwork31010-postgres)
-	[`geonetwork:3.12`](#geonetwork312)
-	[`geonetwork:3.12-postgres`](#geonetwork312-postgres)
-	[`geonetwork:3.12.3`](#geonetwork3123)
-	[`geonetwork:3.12.3-postgres`](#geonetwork3123-postgres)
-	[`geonetwork:4`](#geonetwork4)
-	[`geonetwork:4.0`](#geonetwork40)
-	[`geonetwork:4.0.5`](#geonetwork405)
-	[`geonetwork:latest`](#geonetworklatest)

## `geonetwork:3`

```console
$ docker pull geonetwork@sha256:5d0b62827723a25fd6ce366097ef416aab118b402c95c246350e8488fa16fa0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3` - linux; amd64

```console
$ docker pull geonetwork@sha256:e6033058f72ec11ddd64c8aaed44d80bd566bc830bea22e95f383577d32ee1e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.8 MB (471832723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9d2b49e7f15457b757b838375dbe4dfa00b45edb23acc84d80cd7c1d9f48b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 03:36:40 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:41 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:41 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:37:21 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:37:22 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e4dffd673e2e1861516f501eb6bcf358465df560f59848a0452f298968ccd`  
		Last Modified: Fri, 21 Jan 2022 03:38:44 GMT  
		Size: 223.4 MB (223370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d061ebc7603d626c349b1cb266a00d6e0ae9be83b17f9fe915312f943f82b7`  
		Last Modified: Fri, 21 Jan 2022 03:38:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:5de4c68b540bf821a3849a705b864fee39579ef0e6cbcf3c6cf13aa9a482805e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **469.2 MB (469175416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ac60e7097a65ec531936edea3bb94c3e468444d41534451b69d19ea82a5f26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 04:35:22 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:35:23 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:35:24 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:36:36 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:36:38 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:39 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce0327e906ca83a4bc691953764ac5807f72bfccc1231ede88b891e421197b3`  
		Last Modified: Fri, 21 Jan 2022 04:38:30 GMT  
		Size: 223.4 MB (223369206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c08ba7c0a1c07be66c5098f4fb36d7394abe8acee7aa92cd12399c02e8ac2b`  
		Last Modified: Fri, 21 Jan 2022 04:38:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3-postgres`

```console
$ docker pull geonetwork@sha256:b0e0c830e57e0623fb190e7faa8a26b70cdbd94031b6d7d85359bee058357ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:5769eebb127045dddc90852fb5253e8977717eb94dfe394298c39a447c1fcb73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **475.3 MB (475339922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c5d7d892659d1359ce2e499565b186af72604d24fbf9e6b88e9b6a05359d01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 03:36:40 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:41 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:41 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:37:21 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:37:22 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:22 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:37:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 03:37:33 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 03:37:33 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 03:37:34 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:34 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e4dffd673e2e1861516f501eb6bcf358465df560f59848a0452f298968ccd`  
		Last Modified: Fri, 21 Jan 2022 03:38:44 GMT  
		Size: 223.4 MB (223370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d061ebc7603d626c349b1cb266a00d6e0ae9be83b17f9fe915312f943f82b7`  
		Last Modified: Fri, 21 Jan 2022 03:38:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394541c833cfaba3566cf3d29e641f99d4edfeda667509c07e89dc9585ec8d08`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 3.5 MB (3503826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2631ee82d2282fe59ab0da240e41595c0698efa7d5a1117432bafe1ae1cd8d`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed89437aab312f24153201e7f8ab136defc1ea88c40e4350cc2db563274c7415`  
		Last Modified: Fri, 21 Jan 2022 03:38:58 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3207621ac1be601a817e983bea944614761f14d843e3e837c41cd00498ea16`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:bea99be7537a8d91e357384735daba450b531e6fed9845e17987391574f65a95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.4 MB (472439777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07a2478046444a307dbe02d88013f4b251841d70b60089f298618ce23438696`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 04:35:22 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:35:23 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:35:24 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:36:36 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:36:38 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:39 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:36:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 04:36:52 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 04:36:54 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 04:36:55 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:56 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce0327e906ca83a4bc691953764ac5807f72bfccc1231ede88b891e421197b3`  
		Last Modified: Fri, 21 Jan 2022 04:38:30 GMT  
		Size: 223.4 MB (223369206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c08ba7c0a1c07be66c5098f4fb36d7394abe8acee7aa92cd12399c02e8ac2b`  
		Last Modified: Fri, 21 Jan 2022 04:38:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e71e6023fb812750b8d5a95f2b31055851d41c6868eb824633b661fdc2b0a4`  
		Last Modified: Fri, 21 Jan 2022 04:38:52 GMT  
		Size: 3.3 MB (3260988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0eadad95a9c5084f799ae55222d32d4b9320f79abc4a8511096ce14d108c4d`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485010b3cae85664f1245580b25916c4e94a37d26c7f617f3d19b046139cdf3`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf4edd4623a40bac78ac9ba370c4da93cdad925a2252f11ed67f963a2546440`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10`

```console
$ docker pull geonetwork@sha256:b2ff500b7d1ba5060abcbb80eaf61f2fa1cad639059b97916970e89db9f65103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.10` - linux; amd64

```console
$ docker pull geonetwork@sha256:8875ba228ceec849fe943bb6761199c6a251f6469531e4f0eb8fd52bc746c4a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444118909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555f8c29c0d9fd4be921617ed609871b32845b015f5cf82266d3c002d3bbb5cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:13 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:36:26 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:36:27 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1374e6316b22c138fc1489a14a6dce969704ffc0dd8564219340fb5038bd6`  
		Last Modified: Fri, 21 Jan 2022 03:38:08 GMT  
		Size: 195.7 MB (195657179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9c3e20c0d0d5aa998ce2974f56ba5d43415fb3791ba926cf36e161030a5ba`  
		Last Modified: Fri, 21 Jan 2022 03:37:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.10` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:a1b4b64ae16e001d988a4b18038512326acd679d6337faf608c06575a01af9c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441464812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7608820d0fc432783542544c88dc149d5c7f5f6446dd2ff9f9893b88d0a948e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:33:43 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 04:33:44 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 04:33:45 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:33:46 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:33:47 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:34:53 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:34:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:34:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:34:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be1eaf607f09dabb6a5bc56cc35723ce1187ddcba3ac62c1a9d69545fbabf3`  
		Last Modified: Fri, 21 Jan 2022 04:37:49 GMT  
		Size: 195.7 MB (195658600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88022caa4afafd29ad0927e6b75f42a57fe717d29f7893da555af014d492f0`  
		Last Modified: Fri, 21 Jan 2022 04:37:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10-postgres`

```console
$ docker pull geonetwork@sha256:93ea76cb1c40b31cb69583a403938dadf6b109991267dfee6c9ca038fe738017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.10-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:bace1db17c5c36dc8c06b2b3d0ca550d88efd6e41fee4111dca4d75429ac443e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.6 MB (447626114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3f783fad0eaa665dee7454a5415612358f3c8b71c873167cca01a9618d1d30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:13 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:36:26 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:36:27 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:28 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 03:36:36 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 03:36:37 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 03:36:37 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1374e6316b22c138fc1489a14a6dce969704ffc0dd8564219340fb5038bd6`  
		Last Modified: Fri, 21 Jan 2022 03:38:08 GMT  
		Size: 195.7 MB (195657179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9c3e20c0d0d5aa998ce2974f56ba5d43415fb3791ba926cf36e161030a5ba`  
		Last Modified: Fri, 21 Jan 2022 03:37:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9c9e96c2b1845c44574a7ff3754024cbea18a0d8e3536d11a0e80c356c7852`  
		Last Modified: Fri, 21 Jan 2022 03:38:20 GMT  
		Size: 3.5 MB (3503829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f446c4c757c33d6bba9f70ef10b3791c845b68a4fa1aa7d2982174dec434e`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e7507f5f629388924956e5b89623e275881c93c28ac339ac601497257d4ef7`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb466076f2a463b6d3ce98cf34c6afee63efa2008cfe6869eb93c965489574b3`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.10-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:63ce359559b97ac2f42e5886c178fe1c9f4006d350b9336a0d911dbab78abc0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.7 MB (444729156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c54eb1924ff4415bc8c40dd1b075f3718cbd61ffd4bb4af722845a4f6e1985`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:33:43 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 04:33:44 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 04:33:45 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:33:46 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:33:47 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:34:53 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:34:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:34:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:34:55 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:35:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 04:35:12 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 04:35:13 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 04:35:14 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 04:35:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:35:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be1eaf607f09dabb6a5bc56cc35723ce1187ddcba3ac62c1a9d69545fbabf3`  
		Last Modified: Fri, 21 Jan 2022 04:37:49 GMT  
		Size: 195.7 MB (195658600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88022caa4afafd29ad0927e6b75f42a57fe717d29f7893da555af014d492f0`  
		Last Modified: Fri, 21 Jan 2022 04:37:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36507d7a352dbc43d6ac0c41af1182c3e2673c4cf9799d711a4480d7ead34a1e`  
		Last Modified: Fri, 21 Jan 2022 04:38:02 GMT  
		Size: 3.3 MB (3260969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b05ba9ebecd3da7073e432b800178c2ecfb73472f4c311d8b4a1a5277fdff1`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db519abd8575b7e6a873548c4be53a00a7e889fcc98b8ff6a2228afe9ad376d7`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2108d0d0ec4deb9841b90111420a5075cfcc3178a437d2f9d8a8208df0839d`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10.10`

```console
$ docker pull geonetwork@sha256:b2ff500b7d1ba5060abcbb80eaf61f2fa1cad639059b97916970e89db9f65103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.10.10` - linux; amd64

```console
$ docker pull geonetwork@sha256:8875ba228ceec849fe943bb6761199c6a251f6469531e4f0eb8fd52bc746c4a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444118909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:555f8c29c0d9fd4be921617ed609871b32845b015f5cf82266d3c002d3bbb5cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:13 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:36:26 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:36:27 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1374e6316b22c138fc1489a14a6dce969704ffc0dd8564219340fb5038bd6`  
		Last Modified: Fri, 21 Jan 2022 03:38:08 GMT  
		Size: 195.7 MB (195657179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9c3e20c0d0d5aa998ce2974f56ba5d43415fb3791ba926cf36e161030a5ba`  
		Last Modified: Fri, 21 Jan 2022 03:37:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.10.10` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:a1b4b64ae16e001d988a4b18038512326acd679d6337faf608c06575a01af9c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.5 MB (441464812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7608820d0fc432783542544c88dc149d5c7f5f6446dd2ff9f9893b88d0a948e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:33:43 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 04:33:44 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 04:33:45 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:33:46 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:33:47 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:34:53 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:34:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:34:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:34:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be1eaf607f09dabb6a5bc56cc35723ce1187ddcba3ac62c1a9d69545fbabf3`  
		Last Modified: Fri, 21 Jan 2022 04:37:49 GMT  
		Size: 195.7 MB (195658600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88022caa4afafd29ad0927e6b75f42a57fe717d29f7893da555af014d492f0`  
		Last Modified: Fri, 21 Jan 2022 04:37:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.10.10-postgres`

```console
$ docker pull geonetwork@sha256:93ea76cb1c40b31cb69583a403938dadf6b109991267dfee6c9ca038fe738017
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.10.10-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:bace1db17c5c36dc8c06b2b3d0ca550d88efd6e41fee4111dca4d75429ac443e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.6 MB (447626114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3f783fad0eaa665dee7454a5415612358f3c8b71c873167cca01a9618d1d30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 03:36:12 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:12 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:13 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:36:26 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:36:27 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:28 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 03:36:36 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 03:36:37 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 03:36:37 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 03:36:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:36:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1374e6316b22c138fc1489a14a6dce969704ffc0dd8564219340fb5038bd6`  
		Last Modified: Fri, 21 Jan 2022 03:38:08 GMT  
		Size: 195.7 MB (195657179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9c3e20c0d0d5aa998ce2974f56ba5d43415fb3791ba926cf36e161030a5ba`  
		Last Modified: Fri, 21 Jan 2022 03:37:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9c9e96c2b1845c44574a7ff3754024cbea18a0d8e3536d11a0e80c356c7852`  
		Last Modified: Fri, 21 Jan 2022 03:38:20 GMT  
		Size: 3.5 MB (3503829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f446c4c757c33d6bba9f70ef10b3791c845b68a4fa1aa7d2982174dec434e`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e7507f5f629388924956e5b89623e275881c93c28ac339ac601497257d4ef7`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb466076f2a463b6d3ce98cf34c6afee63efa2008cfe6869eb93c965489574b3`  
		Last Modified: Fri, 21 Jan 2022 03:38:19 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.10.10-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:63ce359559b97ac2f42e5886c178fe1c9f4006d350b9336a0d911dbab78abc0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.7 MB (444729156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c54eb1924ff4415bc8c40dd1b075f3718cbd61ffd4bb4af722845a4f6e1985`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:33:43 GMT
ENV GN_VERSION=3.10.10
# Fri, 21 Jan 2022 04:33:44 GMT
ENV GN_DOWNLOAD_MD5=de09ba1a43d6f3a224ad5ff02b4c4fb3
# Fri, 21 Jan 2022 04:33:45 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:33:46 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:33:47 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:34:53 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "$GN_DOWNLOAD_MD5 *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:34:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:34:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:34:55 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:35:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 04:35:12 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 04:35:13 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 04:35:14 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 04:35:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:35:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6be1eaf607f09dabb6a5bc56cc35723ce1187ddcba3ac62c1a9d69545fbabf3`  
		Last Modified: Fri, 21 Jan 2022 04:37:49 GMT  
		Size: 195.7 MB (195658600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f88022caa4afafd29ad0927e6b75f42a57fe717d29f7893da555af014d492f0`  
		Last Modified: Fri, 21 Jan 2022 04:37:34 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36507d7a352dbc43d6ac0c41af1182c3e2673c4cf9799d711a4480d7ead34a1e`  
		Last Modified: Fri, 21 Jan 2022 04:38:02 GMT  
		Size: 3.3 MB (3260969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b05ba9ebecd3da7073e432b800178c2ecfb73472f4c311d8b4a1a5277fdff1`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db519abd8575b7e6a873548c4be53a00a7e889fcc98b8ff6a2228afe9ad376d7`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2108d0d0ec4deb9841b90111420a5075cfcc3178a437d2f9d8a8208df0839d`  
		Last Modified: Fri, 21 Jan 2022 04:38:01 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12`

```console
$ docker pull geonetwork@sha256:5d0b62827723a25fd6ce366097ef416aab118b402c95c246350e8488fa16fa0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.12` - linux; amd64

```console
$ docker pull geonetwork@sha256:e6033058f72ec11ddd64c8aaed44d80bd566bc830bea22e95f383577d32ee1e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.8 MB (471832723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9d2b49e7f15457b757b838375dbe4dfa00b45edb23acc84d80cd7c1d9f48b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 03:36:40 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:41 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:41 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:37:21 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:37:22 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e4dffd673e2e1861516f501eb6bcf358465df560f59848a0452f298968ccd`  
		Last Modified: Fri, 21 Jan 2022 03:38:44 GMT  
		Size: 223.4 MB (223370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d061ebc7603d626c349b1cb266a00d6e0ae9be83b17f9fe915312f943f82b7`  
		Last Modified: Fri, 21 Jan 2022 03:38:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:5de4c68b540bf821a3849a705b864fee39579ef0e6cbcf3c6cf13aa9a482805e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **469.2 MB (469175416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ac60e7097a65ec531936edea3bb94c3e468444d41534451b69d19ea82a5f26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 04:35:22 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:35:23 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:35:24 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:36:36 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:36:38 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:39 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce0327e906ca83a4bc691953764ac5807f72bfccc1231ede88b891e421197b3`  
		Last Modified: Fri, 21 Jan 2022 04:38:30 GMT  
		Size: 223.4 MB (223369206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c08ba7c0a1c07be66c5098f4fb36d7394abe8acee7aa92cd12399c02e8ac2b`  
		Last Modified: Fri, 21 Jan 2022 04:38:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12-postgres`

```console
$ docker pull geonetwork@sha256:b0e0c830e57e0623fb190e7faa8a26b70cdbd94031b6d7d85359bee058357ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:3.12-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:5769eebb127045dddc90852fb5253e8977717eb94dfe394298c39a447c1fcb73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **475.3 MB (475339922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c5d7d892659d1359ce2e499565b186af72604d24fbf9e6b88e9b6a05359d01`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:01 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:02 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:06:03 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:06:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 22 Dec 2021 17:09:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:09:57 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:09:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:09:58 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:09:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:09:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:29:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 22 Dec 2021 17:29:05 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:23:49 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:23:50 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:24:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:25:00 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:25:00 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:36:11 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 03:36:11 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 03:36:12 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 03:36:40 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 03:36:40 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 03:36:41 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 03:36:41 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 03:37:21 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 03:37:22 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:22 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 03:37:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 03:37:33 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 03:37:33 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 03:37:34 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 03:37:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 03:37:34 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f6fcc5fa5532a1dd793456f64daf954192e0521fd65d42af584d5e2d93f55`  
		Last Modified: Tue, 21 Dec 2021 23:23:07 GMT  
		Size: 5.4 MB (5420005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0879393b07ef5fa816c292b00e3eb4945890bc2a69ab0d1754240cbe9cedf21`  
		Last Modified: Tue, 21 Dec 2021 23:27:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef50c41a74d450f2d708be5971c3ba635ed1a714af7f4fa1497886adb2fa734`  
		Last Modified: Tue, 21 Dec 2021 23:27:56 GMT  
		Size: 106.0 MB (105998986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcabf45ee9019d95fd14f1bb017321da96be445c15901c798147c988f4635e9`  
		Last Modified: Wed, 22 Dec 2021 17:51:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c703e7eb8fdcd08548eb49469468d172fe088e394925843ae243b544dbca4f`  
		Last Modified: Fri, 21 Jan 2022 03:16:50 GMT  
		Size: 11.5 MB (11532042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed754fc88e9f914da948f56ebd03c55014d9ff1357185a85040f5952df808`  
		Last Modified: Fri, 21 Jan 2022 03:16:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e4dffd673e2e1861516f501eb6bcf358465df560f59848a0452f298968ccd`  
		Last Modified: Fri, 21 Jan 2022 03:38:44 GMT  
		Size: 223.4 MB (223370993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d061ebc7603d626c349b1cb266a00d6e0ae9be83b17f9fe915312f943f82b7`  
		Last Modified: Fri, 21 Jan 2022 03:38:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394541c833cfaba3566cf3d29e641f99d4edfeda667509c07e89dc9585ec8d08`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 3.5 MB (3503826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2631ee82d2282fe59ab0da240e41595c0698efa7d5a1117432bafe1ae1cd8d`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed89437aab312f24153201e7f8ab136defc1ea88c40e4350cc2db563274c7415`  
		Last Modified: Fri, 21 Jan 2022 03:38:58 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3207621ac1be601a817e983bea944614761f14d843e3e837c41cd00498ea16`  
		Last Modified: Fri, 21 Jan 2022 03:38:59 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:bea99be7537a8d91e357384735daba450b531e6fed9845e17987391574f65a95
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **472.4 MB (472439777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d07a2478046444a307dbe02d88013f4b251841d70b60089f298618ce23438696`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 20:43:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 21 Dec 2021 20:43:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 20:43:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 21 Dec 2021 20:43:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 21 Dec 2021 20:43:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 20:43:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 21 Dec 2021 21:07:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 21 Dec 2021 21:07:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 21 Jan 2022 02:46:24 GMT
ENV TOMCAT_VERSION=8.5.75
# Fri, 21 Jan 2022 02:46:25 GMT
ENV TOMCAT_SHA512=b86d191506f8a647e3f4505bb7cc095068abb26bb4283562924913606514ce15930a467bd5d20c09b11d785827bf1914ed869b48dfb1c95e9f826e4c8b4e8aaa
# Fri, 21 Jan 2022 02:46:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 21 Jan 2022 02:46:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 02:46:52 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 02:46:53 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:33:40 GMT
ENV GN_FILE=geonetwork.war
# Fri, 21 Jan 2022 04:33:41 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Fri, 21 Jan 2022 04:33:42 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_VERSION=3.12.2
# Fri, 21 Jan 2022 04:35:21 GMT
ENV GN_DOWNLOAD_MD5=669e70d8d490d49811362889ec222192
# Fri, 21 Jan 2022 04:35:22 GMT
ENV LOG4J_VERSION=2.17.1
# Fri, 21 Jan 2022 04:35:23 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Fri, 21 Jan 2022 04:35:24 GMT
WORKDIR /usr/local/tomcat/webapps
# Fri, 21 Jan 2022 04:36:36 GMT
RUN curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE &&      rm geonetwork/WEB-INF/lib/log4j-core-* &&      rm geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/lib/" &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Fri, 21 Jan 2022 04:36:38 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:39 GMT
CMD ["catalina.sh" "run"]
# Fri, 21 Jan 2022 04:36:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 04:36:52 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Fri, 21 Jan 2022 04:36:54 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Fri, 21 Jan 2022 04:36:55 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Fri, 21 Jan 2022 04:36:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Jan 2022 04:36:56 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c966716b8f78e83c86b7295591316faec97ea4cd1cfe396a6345904831016d`  
		Last Modified: Tue, 21 Dec 2021 21:40:19 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2128b01d3d671509fa9a29067c5dc6b3bbebc378d213e8d72a3745042067e399`  
		Last Modified: Fri, 21 Jan 2022 03:50:23 GMT  
		Size: 11.3 MB (11303597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce0327e906ca83a4bc691953764ac5807f72bfccc1231ede88b891e421197b3`  
		Last Modified: Fri, 21 Jan 2022 04:38:30 GMT  
		Size: 223.4 MB (223369206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c08ba7c0a1c07be66c5098f4fb36d7394abe8acee7aa92cd12399c02e8ac2b`  
		Last Modified: Fri, 21 Jan 2022 04:38:12 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e71e6023fb812750b8d5a95f2b31055851d41c6868eb824633b661fdc2b0a4`  
		Last Modified: Fri, 21 Jan 2022 04:38:52 GMT  
		Size: 3.3 MB (3260988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0eadad95a9c5084f799ae55222d32d4b9320f79abc4a8511096ce14d108c4d`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6485010b3cae85664f1245580b25916c4e94a37d26c7f617f3d19b046139cdf3`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf4edd4623a40bac78ac9ba370c4da93cdad925a2252f11ed67f963a2546440`  
		Last Modified: Fri, 21 Jan 2022 04:38:51 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12.3`

**does not exist** (yet?)

## `geonetwork:3.12.3-postgres`

**does not exist** (yet?)

## `geonetwork:4`

```console
$ docker pull geonetwork@sha256:a090e0ac30262030390c2697f08f225265b9d74785032220e5ce5e6af56b4700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4` - linux; amd64

```console
$ docker pull geonetwork@sha256:d9321e6efc23c3535cd28db46ed3446c54ca48b13b7b0f105500cc2c27615985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.9 MB (430867474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d3d6924189372c84af0cd08824eb67381178307209ca7d209bbf67abab31b`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:07:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:07:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:07:31 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:07:32 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:07:32 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Wed, 22 Dec 2021 14:13:10 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Wed, 22 Dec 2021 14:13:10 GMT
WORKDIR /var/lib/jetty
# Wed, 22 Dec 2021 14:13:10 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Wed, 22 Dec 2021 14:13:10 GMT
USER jetty
# Wed, 22 Dec 2021 14:13:11 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 14:13:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Dec 2021 14:13:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 19:06:00 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 19:06:00 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 19:06:01 GMT
USER root
# Wed, 22 Dec 2021 19:06:05 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 19:06:06 GMT
USER jetty
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 19:06:07 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:29:34 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:29:35 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:29:35 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:29:36 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:29:36 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce012bef046180a22ef3146fac08398ed1fec48c7b1609b9aed1801e42dfce`  
		Last Modified: Tue, 21 Dec 2021 23:26:08 GMT  
		Size: 5.7 MB (5653770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dc2a72d098601f2b48898ff5e748c316037366c46e554b830cb90ad15519ba`  
		Last Modified: Tue, 21 Dec 2021 23:29:33 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69a57e10d955041a2cb3ad37236bedbd7ad473dc42d5fa3d88f648affa3a12`  
		Last Modified: Tue, 21 Dec 2021 23:29:39 GMT  
		Size: 41.4 MB (41372029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91e7905f04f436034549ffaf42c1fbc22c54d35d31b778a8c2da4ea24a18d5`  
		Last Modified: Wed, 22 Dec 2021 14:19:26 GMT  
		Size: 9.9 MB (9878319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e69948f83a53246716329d261fb7741848dc923463d9e0ce3bba2643d146df`  
		Last Modified: Wed, 22 Dec 2021 14:19:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b832412035ef18cee30821f5ad7473a587160a8772ed8033a737bc4770e799`  
		Last Modified: Wed, 22 Dec 2021 19:09:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732737ad678ffe9e447c2735d11e7f387850f284979edc1c6fa8f778804862d`  
		Last Modified: Tue, 18 Jan 2022 18:32:23 GMT  
		Size: 303.0 MB (303016513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f479364004d843ef30b98bddf051765f85778462c0e3e54166f1e924deb3a57`  
		Last Modified: Tue, 18 Jan 2022 18:32:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:0af48bc58d1ae235b50ec4f224bc86eaec144430abe035204580bb3d7b8e8a9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.6 MB (428572666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20b61c9e6c4c39a5bc6478f9c96ce305f780e9c420c88b0542b636fb3b65cf7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:05:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:05:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:05:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:06:00 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:06:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 21 Dec 2021 23:51:57 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Tue, 21 Dec 2021 23:51:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 21 Dec 2021 23:51:59 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 21 Dec 2021 23:52:00 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 21 Dec 2021 23:52:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:52:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Tue, 21 Dec 2021 23:52:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 21 Dec 2021 23:52:09 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 21 Dec 2021 23:52:10 GMT
WORKDIR /var/lib/jetty
# Tue, 21 Dec 2021 23:52:12 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 21 Dec 2021 23:52:12 GMT
USER jetty
# Tue, 21 Dec 2021 23:52:13 GMT
EXPOSE 8080
# Tue, 21 Dec 2021 23:52:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:52:15 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 04:40:39 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 04:40:40 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 04:40:41 GMT
USER root
# Wed, 22 Dec 2021 04:40:45 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 04:40:45 GMT
USER jetty
# Wed, 22 Dec 2021 04:40:46 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 04:40:47 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 04:40:48 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:52:48 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:52:49 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:52:49 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:52:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:52:51 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96afb7af5f2665c7daa5679fa4d9b14dadc6f2cf69c90a1f0e5ae35e51f046e`  
		Last Modified: Tue, 21 Dec 2021 03:28:57 GMT  
		Size: 5.6 MB (5647149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b520866ec81d53d5538a95aba935c6c821c4a25901f61ea3be5bf4e759d38608`  
		Last Modified: Tue, 21 Dec 2021 03:32:56 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe53258e8d519a21424fd4d93be71a9076697af867528ffec37a76a5c1ac42d`  
		Last Modified: Tue, 21 Dec 2021 03:33:01 GMT  
		Size: 40.6 MB (40625382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e383aae79b99fe91405c8c4372083fc25cbd1bc388f99e67b15eda84b85ce28`  
		Last Modified: Wed, 22 Dec 2021 00:01:36 GMT  
		Size: 9.9 MB (9878004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c380c9805f8d1f4a483ca00b3d659669b6df093a8e21ee7b1b1593fefbb9f`  
		Last Modified: Wed, 22 Dec 2021 00:01:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76883185f35abeadf8db11647a30ab8ebe9384c27f514d13d17e2d7b7fc4141e`  
		Last Modified: Wed, 22 Dec 2021 04:44:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1fd56254999f8a31fb01a30b6b282b436db673047ad31abb62920ef7eccd5b`  
		Last Modified: Tue, 18 Jan 2022 18:55:24 GMT  
		Size: 303.0 MB (303017271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f126885fb403b3e6586033cef672962dee20d8805b82bc2f700e309c9adcc33`  
		Last Modified: Tue, 18 Jan 2022 18:55:03 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.0`

```console
$ docker pull geonetwork@sha256:a090e0ac30262030390c2697f08f225265b9d74785032220e5ce5e6af56b4700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.0` - linux; amd64

```console
$ docker pull geonetwork@sha256:d9321e6efc23c3535cd28db46ed3446c54ca48b13b7b0f105500cc2c27615985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.9 MB (430867474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d3d6924189372c84af0cd08824eb67381178307209ca7d209bbf67abab31b`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:07:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:07:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:07:31 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:07:32 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:07:32 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Wed, 22 Dec 2021 14:13:10 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Wed, 22 Dec 2021 14:13:10 GMT
WORKDIR /var/lib/jetty
# Wed, 22 Dec 2021 14:13:10 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Wed, 22 Dec 2021 14:13:10 GMT
USER jetty
# Wed, 22 Dec 2021 14:13:11 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 14:13:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Dec 2021 14:13:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 19:06:00 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 19:06:00 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 19:06:01 GMT
USER root
# Wed, 22 Dec 2021 19:06:05 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 19:06:06 GMT
USER jetty
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 19:06:07 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:29:34 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:29:35 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:29:35 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:29:36 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:29:36 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce012bef046180a22ef3146fac08398ed1fec48c7b1609b9aed1801e42dfce`  
		Last Modified: Tue, 21 Dec 2021 23:26:08 GMT  
		Size: 5.7 MB (5653770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dc2a72d098601f2b48898ff5e748c316037366c46e554b830cb90ad15519ba`  
		Last Modified: Tue, 21 Dec 2021 23:29:33 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69a57e10d955041a2cb3ad37236bedbd7ad473dc42d5fa3d88f648affa3a12`  
		Last Modified: Tue, 21 Dec 2021 23:29:39 GMT  
		Size: 41.4 MB (41372029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91e7905f04f436034549ffaf42c1fbc22c54d35d31b778a8c2da4ea24a18d5`  
		Last Modified: Wed, 22 Dec 2021 14:19:26 GMT  
		Size: 9.9 MB (9878319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e69948f83a53246716329d261fb7741848dc923463d9e0ce3bba2643d146df`  
		Last Modified: Wed, 22 Dec 2021 14:19:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b832412035ef18cee30821f5ad7473a587160a8772ed8033a737bc4770e799`  
		Last Modified: Wed, 22 Dec 2021 19:09:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732737ad678ffe9e447c2735d11e7f387850f284979edc1c6fa8f778804862d`  
		Last Modified: Tue, 18 Jan 2022 18:32:23 GMT  
		Size: 303.0 MB (303016513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f479364004d843ef30b98bddf051765f85778462c0e3e54166f1e924deb3a57`  
		Last Modified: Tue, 18 Jan 2022 18:32:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.0` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:0af48bc58d1ae235b50ec4f224bc86eaec144430abe035204580bb3d7b8e8a9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.6 MB (428572666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20b61c9e6c4c39a5bc6478f9c96ce305f780e9c420c88b0542b636fb3b65cf7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:05:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:05:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:05:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:06:00 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:06:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 21 Dec 2021 23:51:57 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Tue, 21 Dec 2021 23:51:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 21 Dec 2021 23:51:59 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 21 Dec 2021 23:52:00 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 21 Dec 2021 23:52:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:52:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Tue, 21 Dec 2021 23:52:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 21 Dec 2021 23:52:09 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 21 Dec 2021 23:52:10 GMT
WORKDIR /var/lib/jetty
# Tue, 21 Dec 2021 23:52:12 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 21 Dec 2021 23:52:12 GMT
USER jetty
# Tue, 21 Dec 2021 23:52:13 GMT
EXPOSE 8080
# Tue, 21 Dec 2021 23:52:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:52:15 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 04:40:39 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 04:40:40 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 04:40:41 GMT
USER root
# Wed, 22 Dec 2021 04:40:45 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 04:40:45 GMT
USER jetty
# Wed, 22 Dec 2021 04:40:46 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 04:40:47 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 04:40:48 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:52:48 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:52:49 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:52:49 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:52:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:52:51 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96afb7af5f2665c7daa5679fa4d9b14dadc6f2cf69c90a1f0e5ae35e51f046e`  
		Last Modified: Tue, 21 Dec 2021 03:28:57 GMT  
		Size: 5.6 MB (5647149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b520866ec81d53d5538a95aba935c6c821c4a25901f61ea3be5bf4e759d38608`  
		Last Modified: Tue, 21 Dec 2021 03:32:56 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe53258e8d519a21424fd4d93be71a9076697af867528ffec37a76a5c1ac42d`  
		Last Modified: Tue, 21 Dec 2021 03:33:01 GMT  
		Size: 40.6 MB (40625382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e383aae79b99fe91405c8c4372083fc25cbd1bc388f99e67b15eda84b85ce28`  
		Last Modified: Wed, 22 Dec 2021 00:01:36 GMT  
		Size: 9.9 MB (9878004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c380c9805f8d1f4a483ca00b3d659669b6df093a8e21ee7b1b1593fefbb9f`  
		Last Modified: Wed, 22 Dec 2021 00:01:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76883185f35abeadf8db11647a30ab8ebe9384c27f514d13d17e2d7b7fc4141e`  
		Last Modified: Wed, 22 Dec 2021 04:44:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1fd56254999f8a31fb01a30b6b282b436db673047ad31abb62920ef7eccd5b`  
		Last Modified: Tue, 18 Jan 2022 18:55:24 GMT  
		Size: 303.0 MB (303017271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f126885fb403b3e6586033cef672962dee20d8805b82bc2f700e309c9adcc33`  
		Last Modified: Tue, 18 Jan 2022 18:55:03 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.0.5`

```console
$ docker pull geonetwork@sha256:a090e0ac30262030390c2697f08f225265b9d74785032220e5ce5e6af56b4700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.0.5` - linux; amd64

```console
$ docker pull geonetwork@sha256:d9321e6efc23c3535cd28db46ed3446c54ca48b13b7b0f105500cc2c27615985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.9 MB (430867474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d3d6924189372c84af0cd08824eb67381178307209ca7d209bbf67abab31b`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:07:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:07:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:07:31 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:07:32 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:07:32 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Wed, 22 Dec 2021 14:13:10 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Wed, 22 Dec 2021 14:13:10 GMT
WORKDIR /var/lib/jetty
# Wed, 22 Dec 2021 14:13:10 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Wed, 22 Dec 2021 14:13:10 GMT
USER jetty
# Wed, 22 Dec 2021 14:13:11 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 14:13:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Dec 2021 14:13:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 19:06:00 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 19:06:00 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 19:06:01 GMT
USER root
# Wed, 22 Dec 2021 19:06:05 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 19:06:06 GMT
USER jetty
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 19:06:07 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:29:34 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:29:35 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:29:35 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:29:36 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:29:36 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce012bef046180a22ef3146fac08398ed1fec48c7b1609b9aed1801e42dfce`  
		Last Modified: Tue, 21 Dec 2021 23:26:08 GMT  
		Size: 5.7 MB (5653770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dc2a72d098601f2b48898ff5e748c316037366c46e554b830cb90ad15519ba`  
		Last Modified: Tue, 21 Dec 2021 23:29:33 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69a57e10d955041a2cb3ad37236bedbd7ad473dc42d5fa3d88f648affa3a12`  
		Last Modified: Tue, 21 Dec 2021 23:29:39 GMT  
		Size: 41.4 MB (41372029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91e7905f04f436034549ffaf42c1fbc22c54d35d31b778a8c2da4ea24a18d5`  
		Last Modified: Wed, 22 Dec 2021 14:19:26 GMT  
		Size: 9.9 MB (9878319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e69948f83a53246716329d261fb7741848dc923463d9e0ce3bba2643d146df`  
		Last Modified: Wed, 22 Dec 2021 14:19:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b832412035ef18cee30821f5ad7473a587160a8772ed8033a737bc4770e799`  
		Last Modified: Wed, 22 Dec 2021 19:09:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732737ad678ffe9e447c2735d11e7f387850f284979edc1c6fa8f778804862d`  
		Last Modified: Tue, 18 Jan 2022 18:32:23 GMT  
		Size: 303.0 MB (303016513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f479364004d843ef30b98bddf051765f85778462c0e3e54166f1e924deb3a57`  
		Last Modified: Tue, 18 Jan 2022 18:32:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.0.5` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:0af48bc58d1ae235b50ec4f224bc86eaec144430abe035204580bb3d7b8e8a9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.6 MB (428572666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20b61c9e6c4c39a5bc6478f9c96ce305f780e9c420c88b0542b636fb3b65cf7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:05:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:05:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:05:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:06:00 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:06:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 21 Dec 2021 23:51:57 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Tue, 21 Dec 2021 23:51:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 21 Dec 2021 23:51:59 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 21 Dec 2021 23:52:00 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 21 Dec 2021 23:52:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:52:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Tue, 21 Dec 2021 23:52:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 21 Dec 2021 23:52:09 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 21 Dec 2021 23:52:10 GMT
WORKDIR /var/lib/jetty
# Tue, 21 Dec 2021 23:52:12 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 21 Dec 2021 23:52:12 GMT
USER jetty
# Tue, 21 Dec 2021 23:52:13 GMT
EXPOSE 8080
# Tue, 21 Dec 2021 23:52:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:52:15 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 04:40:39 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 04:40:40 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 04:40:41 GMT
USER root
# Wed, 22 Dec 2021 04:40:45 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 04:40:45 GMT
USER jetty
# Wed, 22 Dec 2021 04:40:46 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 04:40:47 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 04:40:48 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:52:48 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:52:49 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:52:49 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:52:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:52:51 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96afb7af5f2665c7daa5679fa4d9b14dadc6f2cf69c90a1f0e5ae35e51f046e`  
		Last Modified: Tue, 21 Dec 2021 03:28:57 GMT  
		Size: 5.6 MB (5647149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b520866ec81d53d5538a95aba935c6c821c4a25901f61ea3be5bf4e759d38608`  
		Last Modified: Tue, 21 Dec 2021 03:32:56 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe53258e8d519a21424fd4d93be71a9076697af867528ffec37a76a5c1ac42d`  
		Last Modified: Tue, 21 Dec 2021 03:33:01 GMT  
		Size: 40.6 MB (40625382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e383aae79b99fe91405c8c4372083fc25cbd1bc388f99e67b15eda84b85ce28`  
		Last Modified: Wed, 22 Dec 2021 00:01:36 GMT  
		Size: 9.9 MB (9878004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c380c9805f8d1f4a483ca00b3d659669b6df093a8e21ee7b1b1593fefbb9f`  
		Last Modified: Wed, 22 Dec 2021 00:01:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76883185f35abeadf8db11647a30ab8ebe9384c27f514d13d17e2d7b7fc4141e`  
		Last Modified: Wed, 22 Dec 2021 04:44:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1fd56254999f8a31fb01a30b6b282b436db673047ad31abb62920ef7eccd5b`  
		Last Modified: Tue, 18 Jan 2022 18:55:24 GMT  
		Size: 303.0 MB (303017271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f126885fb403b3e6586033cef672962dee20d8805b82bc2f700e309c9adcc33`  
		Last Modified: Tue, 18 Jan 2022 18:55:03 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:latest`

```console
$ docker pull geonetwork@sha256:a090e0ac30262030390c2697f08f225265b9d74785032220e5ce5e6af56b4700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:latest` - linux; amd64

```console
$ docker pull geonetwork@sha256:d9321e6efc23c3535cd28db46ed3446c54ca48b13b7b0f105500cc2c27615985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **430.9 MB (430867474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d3d6924189372c84af0cd08824eb67381178307209ca7d209bbf67abab31b`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:04:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:07:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:07:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:07:31 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:07:32 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:07:32 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:07:43 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Wed, 22 Dec 2021 14:13:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV TMPDIR=/tmp/jetty
# Wed, 22 Dec 2021 14:13:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Wed, 22 Dec 2021 14:13:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Wed, 22 Dec 2021 14:13:10 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Wed, 22 Dec 2021 14:13:10 GMT
WORKDIR /var/lib/jetty
# Wed, 22 Dec 2021 14:13:10 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Wed, 22 Dec 2021 14:13:10 GMT
USER jetty
# Wed, 22 Dec 2021 14:13:11 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 14:13:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Dec 2021 14:13:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 19:06:00 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 19:06:00 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 19:06:01 GMT
USER root
# Wed, 22 Dec 2021 19:06:05 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 19:06:06 GMT
USER jetty
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 19:06:06 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 19:06:07 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:28:00 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:29:34 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:29:35 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:29:35 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:29:36 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:29:36 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce012bef046180a22ef3146fac08398ed1fec48c7b1609b9aed1801e42dfce`  
		Last Modified: Tue, 21 Dec 2021 23:26:08 GMT  
		Size: 5.7 MB (5653770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dc2a72d098601f2b48898ff5e748c316037366c46e554b830cb90ad15519ba`  
		Last Modified: Tue, 21 Dec 2021 23:29:33 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69a57e10d955041a2cb3ad37236bedbd7ad473dc42d5fa3d88f648affa3a12`  
		Last Modified: Tue, 21 Dec 2021 23:29:39 GMT  
		Size: 41.4 MB (41372029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf91e7905f04f436034549ffaf42c1fbc22c54d35d31b778a8c2da4ea24a18d5`  
		Last Modified: Wed, 22 Dec 2021 14:19:26 GMT  
		Size: 9.9 MB (9878319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e69948f83a53246716329d261fb7741848dc923463d9e0ce3bba2643d146df`  
		Last Modified: Wed, 22 Dec 2021 14:19:25 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b832412035ef18cee30821f5ad7473a587160a8772ed8033a737bc4770e799`  
		Last Modified: Wed, 22 Dec 2021 19:09:36 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732737ad678ffe9e447c2735d11e7f387850f284979edc1c6fa8f778804862d`  
		Last Modified: Tue, 18 Jan 2022 18:32:23 GMT  
		Size: 303.0 MB (303016513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f479364004d843ef30b98bddf051765f85778462c0e3e54166f1e924deb3a57`  
		Last Modified: Tue, 18 Jan 2022 18:32:04 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:latest` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:0af48bc58d1ae235b50ec4f224bc86eaec144430abe035204580bb3d7b8e8a9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.6 MB (428572666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20b61c9e6c4c39a5bc6478f9c96ce305f780e9c420c88b0542b636fb3b65cf7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:05:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:05:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:05:58 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:05:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:06:00 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:06:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 21 Dec 2021 23:51:57 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Tue, 21 Dec 2021 23:51:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 21 Dec 2021 23:51:59 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 21 Dec 2021 23:52:00 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 21 Dec 2021 23:52:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:52:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Tue, 21 Dec 2021 23:52:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 21 Dec 2021 23:52:09 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 21 Dec 2021 23:52:10 GMT
WORKDIR /var/lib/jetty
# Tue, 21 Dec 2021 23:52:12 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 21 Dec 2021 23:52:12 GMT
USER jetty
# Tue, 21 Dec 2021 23:52:13 GMT
EXPOSE 8080
# Tue, 21 Dec 2021 23:52:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:52:15 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Wed, 22 Dec 2021 04:40:39 GMT
ENV DATA_DIR=/catalogue-data
# Wed, 22 Dec 2021 04:40:40 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Wed, 22 Dec 2021 04:40:41 GMT
USER root
# Wed, 22 Dec 2021 04:40:45 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Wed, 22 Dec 2021 04:40:45 GMT
USER jetty
# Wed, 22 Dec 2021 04:40:46 GMT
ENV GN_FILE=GeoNetwork-4.0.5-0.war
# Wed, 22 Dec 2021 04:40:47 GMT
ENV GN_VERSION=4.0.5
# Wed, 22 Dec 2021 04:40:48 GMT
ENV GN_DOWNLOAD_MD5=7dfcfdffc66b9a97f0d24b0769e9c3b7
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_VERSION=2.17.1
# Tue, 18 Jan 2022 18:48:11 GMT
ENV LOG4J_SHA512=b7e948df6c6f57d903d990de2cc0270c1537b711285e9b6b91280db6ace38418fced713785b2c20512dd9a4238c2d1d0ceb414d9936df2ca110ff14993ae04dc
# Tue, 18 Jan 2022 18:52:48 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-core-* &&      rm /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/log4j-api* &&      curl -fSL -o apache-log4j-${LOG4J_VERSION}-bin.tar.gz "https://dlcdn.apache.org/logging/log4j/${LOG4J_VERSION}/apache-log4j-${LOG4J_VERSION}-bin.tar.gz" &&      echo "${LOG4J_SHA512} apache-log4j-${LOG4J_VERSION}-bin.tar.gz" | sha512sum -c &&      tar -xvzf apache-log4j-${LOG4J_VERSION}-bin.tar.gz &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-core-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      cp apache-log4j-${LOG4J_VERSION}-bin/log4j-api-${LOG4J_VERSION}.jar /var/lib/jetty/webapps/geonetwork/WEB-INF/lib/ &&      rm -rf apache-log4j-${LOG4J_VERSION}-bin*
# Tue, 18 Jan 2022 18:52:49 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 18 Jan 2022 18:52:49 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 18 Jan 2022 18:52:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 18 Jan 2022 18:52:51 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96afb7af5f2665c7daa5679fa4d9b14dadc6f2cf69c90a1f0e5ae35e51f046e`  
		Last Modified: Tue, 21 Dec 2021 03:28:57 GMT  
		Size: 5.6 MB (5647149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b520866ec81d53d5538a95aba935c6c821c4a25901f61ea3be5bf4e759d38608`  
		Last Modified: Tue, 21 Dec 2021 03:32:56 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe53258e8d519a21424fd4d93be71a9076697af867528ffec37a76a5c1ac42d`  
		Last Modified: Tue, 21 Dec 2021 03:33:01 GMT  
		Size: 40.6 MB (40625382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e383aae79b99fe91405c8c4372083fc25cbd1bc388f99e67b15eda84b85ce28`  
		Last Modified: Wed, 22 Dec 2021 00:01:36 GMT  
		Size: 9.9 MB (9878004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68c380c9805f8d1f4a483ca00b3d659669b6df093a8e21ee7b1b1593fefbb9f`  
		Last Modified: Wed, 22 Dec 2021 00:01:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76883185f35abeadf8db11647a30ab8ebe9384c27f514d13d17e2d7b7fc4141e`  
		Last Modified: Wed, 22 Dec 2021 04:44:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1fd56254999f8a31fb01a30b6b282b436db673047ad31abb62920ef7eccd5b`  
		Last Modified: Tue, 18 Jan 2022 18:55:24 GMT  
		Size: 303.0 MB (303017271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f126885fb403b3e6586033cef672962dee20d8805b82bc2f700e309c9adcc33`  
		Last Modified: Tue, 18 Jan 2022 18:55:03 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
