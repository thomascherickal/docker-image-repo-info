<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `geonetwork`

-	[`geonetwork:3`](#geonetwork3)
-	[`geonetwork:3-postgres`](#geonetwork3-postgres)
-	[`geonetwork:3.12`](#geonetwork312)
-	[`geonetwork:3.12-postgres`](#geonetwork312-postgres)
-	[`geonetwork:3.12.11`](#geonetwork31211)
-	[`geonetwork:3.12.11-postgres`](#geonetwork31211-postgres)
-	[`geonetwork:4`](#geonetwork4)
-	[`geonetwork:4.2`](#geonetwork42)
-	[`geonetwork:4.2.7`](#geonetwork427)
-	[`geonetwork:4.4`](#geonetwork44)
-	[`geonetwork:4.4.1`](#geonetwork441)
-	[`geonetwork:latest`](#geonetworklatest)

## `geonetwork:3`

```console
$ docker pull geonetwork@sha256:a3a59ae248c1512d74b7f96da09f4b2c2e6ea84d038eb3e0fda3e74d302d0994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3` - linux; amd64

```console
$ docker pull geonetwork@sha256:f410ac848585cfcc0f0a07b3fc83f3135170399a4beaab6250d1066b1b541cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.6 MB (393567706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846d4002f22864d34336c2b8e98b2c644b691fbcf732e9d0f4aedec4069fc26c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 08:32:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 08:32:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 08:32:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 08:32:43 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 08:32:43 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 08:32:43 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 13:12:25 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:12:25 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 13:12:25 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:12:25 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 13:12:26 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 13:12:26 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 13:12:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 13:12:53 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 13:12:53 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 13:12:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 13:12:53 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720cc92093093d3d4dc588dabcfb301f32a117d9d379436f09816dbf37b2e89`  
		Last Modified: Sat, 02 Dec 2023 08:47:36 GMT  
		Size: 11.8 MB (11843052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af9119b9419708b3b0f6ea386373708353ab7a8a9f9adf10bef66d1f80e9e3c`  
		Last Modified: Sat, 02 Dec 2023 08:47:34 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1ca4e458b13f39322f066cf7cb45b1c4ca9d10fe19459b04d73fad54a0185d`  
		Last Modified: Sat, 02 Dec 2023 13:18:45 GMT  
		Size: 234.8 MB (234776265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d59f8f7d463530bc162f646b92de36663f77be3ca9081aaf6260c15f9acb42b`  
		Last Modified: Sat, 02 Dec 2023 13:18:32 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:448b6b176beacd2afc73b9ad9bf6abb20d949af41be63029757a4afaba0bc367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.7 MB (390742232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438fef475c5fc62c924cb67338d41a164bfc5be84d673735236bec8ba16a69df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:47baf725d2b8cddf0f4091a8c718ddeeb65d8a1cef8de29427dcbe11656b90a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395447334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d93d62aacd8077b34560b462c018548aa2979e616ef7562e2a7602d4acdd87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:ad62057742e4dcb579b4f51e70670a7fb67e726a15d408a77d2934df368a0725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.2 MB (397217467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6365e65054a5e6817d0c78aca5e21e85f8a1569041361be01f411bd4a3c707d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3-postgres`

```console
$ docker pull geonetwork@sha256:a402f1ff8720abf2ad221c7c6e98e53c96aa4e00b356277d8aa7ed97bf561be1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:6790e77d4af103baf992e2407026a651234160cd3b35abb068f834b37d8b57c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.3 MB (407268289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46090fe889edf02fe95e91983b72ea71c575e74374e528cec87b0be7859a243`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 08:32:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 08:32:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 08:32:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 08:32:43 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 08:32:43 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 08:32:43 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 13:12:25 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:12:25 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 13:12:25 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:12:25 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 13:12:26 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 13:12:26 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 13:12:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 13:12:53 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 13:12:53 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 13:12:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 13:12:53 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 13:13:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 13:13:18 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Sat, 02 Dec 2023 13:13:18 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 02 Dec 2023 13:13:18 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 02 Dec 2023 13:13:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 13:13:18 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5720cc92093093d3d4dc588dabcfb301f32a117d9d379436f09816dbf37b2e89`  
		Last Modified: Sat, 02 Dec 2023 08:47:36 GMT  
		Size: 11.8 MB (11843052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af9119b9419708b3b0f6ea386373708353ab7a8a9f9adf10bef66d1f80e9e3c`  
		Last Modified: Sat, 02 Dec 2023 08:47:34 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1ca4e458b13f39322f066cf7cb45b1c4ca9d10fe19459b04d73fad54a0185d`  
		Last Modified: Sat, 02 Dec 2023 13:18:45 GMT  
		Size: 234.8 MB (234776265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d59f8f7d463530bc162f646b92de36663f77be3ca9081aaf6260c15f9acb42b`  
		Last Modified: Sat, 02 Dec 2023 13:18:32 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59d296f9156369be68c661dc80e93ab7ddca7d99c52d55e0b7c9e5071d77d14`  
		Last Modified: Sat, 02 Dec 2023 13:18:59 GMT  
		Size: 13.7 MB (13697221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a8225bc4d06883333631985496b793f0901e1f55504ea45ff5140f9bdda89b`  
		Last Modified: Sat, 02 Dec 2023 13:18:57 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac11c440b9ec33c65a0737cd0d79f29efbba57ead6ab4ac881a0583ff54b1bcf`  
		Last Modified: Sat, 02 Dec 2023 13:18:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9945d65fdd21dfd2aa647c83f68aeb29c15ac446f014ffbd596c9c17fa7bd6`  
		Last Modified: Sat, 02 Dec 2023 13:18:57 GMT  
		Size: 974.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3-postgres` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:f3a20dd8378e244add56112e0018db707a0ded57555d7d7497b5533b05b2632c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403500957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc374971bab7d7cf27868940f1a3a7f20e5fa3f4d3e1e791b13d479862842c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 01:48:54 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 01:48:54 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 01:48:55 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b097b819d04ba4fdd69be7543f3b8705600d43d4dc4d80720bbfde898b865c`  
		Last Modified: Wed, 13 Dec 2023 01:49:36 GMT  
		Size: 12.8 MB (12755362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c4f78dc9be7269f702aae2535e40a09cad5ee40c6fa17d6884efe41fad3ae5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b0a5ac52a75c82419bf9dea8327da316cd8cd6d97e5a5329c34f4995ea6aa6`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4f4ae83fb747417007570299f307e1ab59a463df67554fee19ad4ce53e8ce5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:b8c8db19922a778b4d9d71b5cd5230c1f9100322577df95c7e3b3bdf09f78067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.1 MB (409051004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a8d8991521d3b0fac25673809aedf4be741480c00195818f4aa4a11da655996`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 03:06:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 03:06:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:06:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8875427bb81d31fb6350053daf929e49b7b5bddcfb8f849553bb862d26a2e0`  
		Last Modified: Wed, 13 Dec 2023 03:06:59 GMT  
		Size: 13.6 MB (13600315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc12737831c1ef7e44c0c46cb11197fc953e0c5268264671d55ab3748619764`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b64ed7620e9b42494093f48e23c935f04a2c7800e2ac063118bd90580d167`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d55dff1a0361827e2edef6886d87cd71a9c76adeda1282196952d869bddb7d`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3-postgres` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:9db06fcf9ca87aba4305064c2458c0f9f3194d1d0ecfc08dc9da0a27def57ee7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.4 MB (411412373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231550a32a8924e94a329e0a9046129366f8a28e89eeceafe87c9cf3ffe81004`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 11:28:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Sat, 02 Dec 2023 11:28:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 02 Dec 2023 11:28:21 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 02 Dec 2023 11:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:28:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284724368be3e305ebd028f7302b24eaf424ae4e40fe163deceaf249dcc129c0`  
		Last Modified: Sat, 02 Dec 2023 11:29:04 GMT  
		Size: 14.2 MB (14191549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723ce2467d25e6aafcc85096e3e66b16dc0c68698b4fcc099346c4132cabb9d0`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7eedc2e35e020336f212e7af54e4a3f92626d1f1d2dee784360e75de85c36a`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eaf4c970558800ce1acbf0c774077201b0bfd0135b6b71e518027cde2672b7`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12`

```console
$ docker pull geonetwork@sha256:ca04bbdbf3e0126c77242aadd6bddd7521655bc1954be3039e51ea6807cb0566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3.12` - linux; amd64

```console
$ docker pull geonetwork@sha256:ba25757614bc6fb88ce90ea2a7724874580aa54a087ec057cb464ee4e15f44eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.5 MB (399530580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b694c07030e2358d97bd59a8cdc9fd44f8d99568d706559c1109b0ce080c6726`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:17:45 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:17:46 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:18:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:18:33 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:18:33 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:18:33 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:20:51 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:20:51 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:20:51 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:21:09 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:21:10 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:21:10 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:21:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459003ea6b1b6f8b0461855679767a090ba2aba62024d514d2ed8420532842d3`  
		Last Modified: Wed, 13 Dec 2023 02:38:17 GMT  
		Size: 17.8 MB (17805465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6aa37b074c9d9ea9871ae6bb2738b0432790966ced0d33761421ddcf08587a`  
		Last Modified: Wed, 13 Dec 2023 02:38:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bbf77ad6f0014d6b37ba6fecd4054db4f851c6288e14b922caedd847597577`  
		Last Modified: Wed, 13 Dec 2023 03:22:40 GMT  
		Size: 234.8 MB (234776727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98bfcaed2bb3e2bd61df4a3e375f11ebd222de40bb6a436d8cf7c6f071d739e`  
		Last Modified: Wed, 13 Dec 2023 03:22:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:448b6b176beacd2afc73b9ad9bf6abb20d949af41be63029757a4afaba0bc367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.7 MB (390742232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438fef475c5fc62c924cb67338d41a164bfc5be84d673735236bec8ba16a69df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:47baf725d2b8cddf0f4091a8c718ddeeb65d8a1cef8de29427dcbe11656b90a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395447334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d93d62aacd8077b34560b462c018548aa2979e616ef7562e2a7602d4acdd87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:ad62057742e4dcb579b4f51e70670a7fb67e726a15d408a77d2934df368a0725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.2 MB (397217467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6365e65054a5e6817d0c78aca5e21e85f8a1569041361be01f411bd4a3c707d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12-postgres`

```console
$ docker pull geonetwork@sha256:de4a39d37e2fe1ea7a9f6839b7e263ced2d6aa39835967d8a7c843b30bf94960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3.12-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:b569386d978ab18569ccee14576d95e1b7451f1c046650425b565d4c5f4df43b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.2 MB (413231954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe4e5ad49217353845345f5c3c2fe2956779f72183d94823a97b6fe4018b4f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:17:45 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:17:46 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:18:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:18:33 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:18:33 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:18:33 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:20:51 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:20:51 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:20:51 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:21:09 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:21:10 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:21:10 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:21:10 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 03:22:08 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 03:22:08 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 03:22:08 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 03:22:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:22:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459003ea6b1b6f8b0461855679767a090ba2aba62024d514d2ed8420532842d3`  
		Last Modified: Wed, 13 Dec 2023 02:38:17 GMT  
		Size: 17.8 MB (17805465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6aa37b074c9d9ea9871ae6bb2738b0432790966ced0d33761421ddcf08587a`  
		Last Modified: Wed, 13 Dec 2023 02:38:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bbf77ad6f0014d6b37ba6fecd4054db4f851c6288e14b922caedd847597577`  
		Last Modified: Wed, 13 Dec 2023 03:22:40 GMT  
		Size: 234.8 MB (234776727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98bfcaed2bb3e2bd61df4a3e375f11ebd222de40bb6a436d8cf7c6f071d739e`  
		Last Modified: Wed, 13 Dec 2023 03:22:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b5e59db7bf28535dd0e4e70a4806b6e08c169bc60ff2f0cbece62ba94c98c1`  
		Last Modified: Wed, 13 Dec 2023 03:22:54 GMT  
		Size: 13.7 MB (13698016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1330e707d796177ec7592e170d882c8b8ba591368c5e5a47992ce5ad75d521`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8088d668b3528e061d88aaa0a00855cec77e3dcb561e990faa735478516f016f`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf52d1c93ac4ba7b2036e03d1977890ba696c1e9aead8a86d3a82bf959c55a5c`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 971.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12-postgres` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:f3a20dd8378e244add56112e0018db707a0ded57555d7d7497b5533b05b2632c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403500957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc374971bab7d7cf27868940f1a3a7f20e5fa3f4d3e1e791b13d479862842c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 01:48:54 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 01:48:54 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 01:48:55 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b097b819d04ba4fdd69be7543f3b8705600d43d4dc4d80720bbfde898b865c`  
		Last Modified: Wed, 13 Dec 2023 01:49:36 GMT  
		Size: 12.8 MB (12755362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c4f78dc9be7269f702aae2535e40a09cad5ee40c6fa17d6884efe41fad3ae5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b0a5ac52a75c82419bf9dea8327da316cd8cd6d97e5a5329c34f4995ea6aa6`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4f4ae83fb747417007570299f307e1ab59a463df67554fee19ad4ce53e8ce5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:b8c8db19922a778b4d9d71b5cd5230c1f9100322577df95c7e3b3bdf09f78067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.1 MB (409051004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a8d8991521d3b0fac25673809aedf4be741480c00195818f4aa4a11da655996`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 03:06:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 03:06:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:06:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8875427bb81d31fb6350053daf929e49b7b5bddcfb8f849553bb862d26a2e0`  
		Last Modified: Wed, 13 Dec 2023 03:06:59 GMT  
		Size: 13.6 MB (13600315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc12737831c1ef7e44c0c46cb11197fc953e0c5268264671d55ab3748619764`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b64ed7620e9b42494093f48e23c935f04a2c7800e2ac063118bd90580d167`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d55dff1a0361827e2edef6886d87cd71a9c76adeda1282196952d869bddb7d`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12-postgres` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:9db06fcf9ca87aba4305064c2458c0f9f3194d1d0ecfc08dc9da0a27def57ee7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.4 MB (411412373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231550a32a8924e94a329e0a9046129366f8a28e89eeceafe87c9cf3ffe81004`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 11:28:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Sat, 02 Dec 2023 11:28:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 02 Dec 2023 11:28:21 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 02 Dec 2023 11:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:28:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284724368be3e305ebd028f7302b24eaf424ae4e40fe163deceaf249dcc129c0`  
		Last Modified: Sat, 02 Dec 2023 11:29:04 GMT  
		Size: 14.2 MB (14191549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723ce2467d25e6aafcc85096e3e66b16dc0c68698b4fcc099346c4132cabb9d0`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7eedc2e35e020336f212e7af54e4a3f92626d1f1d2dee784360e75de85c36a`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eaf4c970558800ce1acbf0c774077201b0bfd0135b6b71e518027cde2672b7`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12.11`

```console
$ docker pull geonetwork@sha256:ca04bbdbf3e0126c77242aadd6bddd7521655bc1954be3039e51ea6807cb0566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3.12.11` - linux; amd64

```console
$ docker pull geonetwork@sha256:ba25757614bc6fb88ce90ea2a7724874580aa54a087ec057cb464ee4e15f44eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.5 MB (399530580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b694c07030e2358d97bd59a8cdc9fd44f8d99568d706559c1109b0ce080c6726`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:17:45 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:17:46 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:18:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:18:33 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:18:33 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:18:33 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:20:51 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:20:51 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:20:51 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:21:09 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:21:10 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:21:10 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:21:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459003ea6b1b6f8b0461855679767a090ba2aba62024d514d2ed8420532842d3`  
		Last Modified: Wed, 13 Dec 2023 02:38:17 GMT  
		Size: 17.8 MB (17805465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6aa37b074c9d9ea9871ae6bb2738b0432790966ced0d33761421ddcf08587a`  
		Last Modified: Wed, 13 Dec 2023 02:38:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bbf77ad6f0014d6b37ba6fecd4054db4f851c6288e14b922caedd847597577`  
		Last Modified: Wed, 13 Dec 2023 03:22:40 GMT  
		Size: 234.8 MB (234776727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98bfcaed2bb3e2bd61df4a3e375f11ebd222de40bb6a436d8cf7c6f071d739e`  
		Last Modified: Wed, 13 Dec 2023 03:22:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:448b6b176beacd2afc73b9ad9bf6abb20d949af41be63029757a4afaba0bc367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.7 MB (390742232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438fef475c5fc62c924cb67338d41a164bfc5be84d673735236bec8ba16a69df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:47baf725d2b8cddf0f4091a8c718ddeeb65d8a1cef8de29427dcbe11656b90a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.4 MB (395447334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d93d62aacd8077b34560b462c018548aa2979e616ef7562e2a7602d4acdd87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:ad62057742e4dcb579b4f51e70670a7fb67e726a15d408a77d2934df368a0725
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.2 MB (397217467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6365e65054a5e6817d0c78aca5e21e85f8a1569041361be01f411bd4a3c707d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:3.12.11-postgres`

```console
$ docker pull geonetwork@sha256:de4a39d37e2fe1ea7a9f6839b7e263ced2d6aa39835967d8a7c843b30bf94960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `geonetwork:3.12.11-postgres` - linux; amd64

```console
$ docker pull geonetwork@sha256:b569386d978ab18569ccee14576d95e1b7451f1c046650425b565d4c5f4df43b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.2 MB (413231954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fe4e5ad49217353845345f5c3c2fe2956779f72183d94823a97b6fe4018b4f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:58:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:58:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:58:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:58:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:58:34 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:40 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:25:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:25:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:25:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:25:03 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:25:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:25:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:32:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:32:09 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:17:45 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:17:46 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:18:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:18:33 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:18:33 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:18:33 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:20:51 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:20:51 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:20:51 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:20:51 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:21:09 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:21:10 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:21:10 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:21:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:21:10 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:22:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 03:22:08 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 03:22:08 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 03:22:08 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 03:22:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:22:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0dd4e5224ba77a5588baadfd0a49dbe1c202ba2c6eaab5e29c7a2904e8718`  
		Last Modified: Sat, 02 Dec 2023 02:03:43 GMT  
		Size: 12.9 MB (12902809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03441d1d9cced70c526fd4b59bf8378ecc812353ce58371d91abcb630b3b0401`  
		Last Modified: Sat, 02 Dec 2023 02:03:49 GMT  
		Size: 103.6 MB (103597812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db162541c53c683418ae5238665c2f116963601165bb62f3256c3fe77355c7bd`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7b8015b57912cf43c00c1d0691d32b04b757e40b1b33374ce19c6e3b5f4f50`  
		Last Modified: Sat, 02 Dec 2023 02:03:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef88638cd7c70752e7ac655ca80493659ad362b5e6630c615468346a90d23c89`  
		Last Modified: Sat, 02 Dec 2023 08:43:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459003ea6b1b6f8b0461855679767a090ba2aba62024d514d2ed8420532842d3`  
		Last Modified: Wed, 13 Dec 2023 02:38:17 GMT  
		Size: 17.8 MB (17805465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6aa37b074c9d9ea9871ae6bb2738b0432790966ced0d33761421ddcf08587a`  
		Last Modified: Wed, 13 Dec 2023 02:38:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bbf77ad6f0014d6b37ba6fecd4054db4f851c6288e14b922caedd847597577`  
		Last Modified: Wed, 13 Dec 2023 03:22:40 GMT  
		Size: 234.8 MB (234776727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98bfcaed2bb3e2bd61df4a3e375f11ebd222de40bb6a436d8cf7c6f071d739e`  
		Last Modified: Wed, 13 Dec 2023 03:22:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b5e59db7bf28535dd0e4e70a4806b6e08c169bc60ff2f0cbece62ba94c98c1`  
		Last Modified: Wed, 13 Dec 2023 03:22:54 GMT  
		Size: 13.7 MB (13698016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1330e707d796177ec7592e170d882c8b8ba591368c5e5a47992ce5ad75d521`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8088d668b3528e061d88aaa0a00855cec77e3dcb561e990faa735478516f016f`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf52d1c93ac4ba7b2036e03d1977890ba696c1e9aead8a86d3a82bf959c55a5c`  
		Last Modified: Wed, 13 Dec 2023 03:22:51 GMT  
		Size: 971.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11-postgres` - linux; arm variant v7

```console
$ docker pull geonetwork@sha256:f3a20dd8378e244add56112e0018db707a0ded57555d7d7497b5533b05b2632c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.5 MB (403500957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc374971bab7d7cf27868940f1a3a7f20e5fa3f4d3e1e791b13d479862842c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:58:40 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:58:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:58:41 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:58:44 GMT
ADD file:852469f16f85d8eff83511eb82d6d4409a4608b882c1634281a43c1c481f70c0 in / 
# Fri, 01 Dec 2023 07:58:44 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:52:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:52:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:52:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:53:15 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:53:16 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:53:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:53:27 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:53:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:53:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 08:16:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 08:16:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 08:16:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 08:16:38 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 08:16:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:16:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 08:21:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 08:21:15 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 01:18:01 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 01:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 01:18:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 01:18:37 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 01:18:37 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 01:18:37 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 01:47:47 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 01:47:47 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 01:47:47 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 01:47:48 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 01:48:39 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 01:48:41 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 01:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:41 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 01:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 01:48:54 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 01:48:54 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 01:48:55 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 01:48:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 01:48:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24265e8b291700ac2b80b990af5be5827ef3d9ba54e498a6e36563c879970e0f`  
		Last Modified: Wed, 29 Nov 2023 22:33:38 GMT  
		Size: 27.5 MB (27523678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca56cd7c50818a0ddad15a810796d44bf99dd0578c20198db6da1751082578f`  
		Last Modified: Sat, 02 Dec 2023 06:56:43 GMT  
		Size: 12.5 MB (12492095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbcc59d02fcf8b162e520045215d64d3d67670c95063acd163c538296ddb089`  
		Last Modified: Sat, 02 Dec 2023 06:56:50 GMT  
		Size: 99.2 MB (99234952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818f69b81acd851c7c51262889eefcae84ec9226046c9a96516236feed9d03da`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf57bf76f082cf1fa0a047d56c9736992d7ac258f12b4767dff65b544cee72`  
		Last Modified: Sat, 02 Dec 2023 06:56:40 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cf6a49eb80cd1641e9b772b70f036ca9abe3c491c21309bf811617a938788e`  
		Last Modified: Sat, 02 Dec 2023 08:28:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ca439272815f11681f9c1f3008e5097e2f92d05056885c001b9794c8c109f7`  
		Last Modified: Wed, 13 Dec 2023 01:29:52 GMT  
		Size: 16.7 MB (16721382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a08306fdd52868b5f736f689be3859974b6d40472decc792d2fdf3425ec029`  
		Last Modified: Wed, 13 Dec 2023 01:29:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f679685c8ec79dfe84e781f849aa6f6ecbc94739e79a9e0d171e0d466814b`  
		Last Modified: Wed, 13 Dec 2023 01:49:21 GMT  
		Size: 234.8 MB (234768677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51f077af8ed5f220e7e246c4dfd954d16c9f991c451a40ab41f47ad5b46865`  
		Last Modified: Wed, 13 Dec 2023 01:49:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b097b819d04ba4fdd69be7543f3b8705600d43d4dc4d80720bbfde898b865c`  
		Last Modified: Wed, 13 Dec 2023 01:49:36 GMT  
		Size: 12.8 MB (12755362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c4f78dc9be7269f702aae2535e40a09cad5ee40c6fa17d6884efe41fad3ae5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b0a5ac52a75c82419bf9dea8327da316cd8cd6d97e5a5329c34f4995ea6aa6`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4f4ae83fb747417007570299f307e1ab59a463df67554fee19ad4ce53e8ce5`  
		Last Modified: Wed, 13 Dec 2023 01:49:34 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11-postgres` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:b8c8db19922a778b4d9d71b5cd5230c1f9100322577df95c7e3b3bdf09f78067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.1 MB (409051004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a8d8991521d3b0fac25673809aedf4be741480c00195818f4aa4a11da655996`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:31:08 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:09 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:31:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:31:14 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:32:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:32:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:32:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:32:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:32:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:37:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:37:57 GMT
ENV TOMCAT_MAJOR=8
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_VERSION=8.5.97
# Wed, 13 Dec 2023 02:07:58 GMT
ENV TOMCAT_SHA512=344ea91c95677fdc243bc58a1f8ab745117a80c0a458ae2e26ebc4f968e06c4bfffaf9a4aae52de3d72b945b05b6e03b7cfae98596c222cbe7d394d52363da86
# Wed, 13 Dec 2023 02:08:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 13 Dec 2023 02:08:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Dec 2023 02:08:31 GMT
EXPOSE 8080
# Wed, 13 Dec 2023 02:08:31 GMT
ENTRYPOINT []
# Wed, 13 Dec 2023 02:08:31 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_FILE=geonetwork.war
# Wed, 13 Dec 2023 03:04:17 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Wed, 13 Dec 2023 03:04:17 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_VERSION=3.12.11
# Wed, 13 Dec 2023 03:04:17 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Wed, 13 Dec 2023 03:04:17 GMT
WORKDIR /usr/local/tomcat/webapps
# Wed, 13 Dec 2023 03:05:52 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Wed, 13 Dec 2023 03:05:54 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Wed, 13 Dec 2023 03:05:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Dec 2023 03:05:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:05:55 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Dec 2023 03:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 03:06:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Wed, 13 Dec 2023 03:06:20 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Wed, 13 Dec 2023 03:06:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Dec 2023 03:06:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd693e5b74a77728d853339f783bee254c5de7b0f35f20b69c65c278bcb0753`  
		Last Modified: Sat, 02 Dec 2023 05:34:59 GMT  
		Size: 12.8 MB (12844949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48442aadc321fe3bd68398c80b79d23a86f3c43520c1355c0ebcd8202d40df5b`  
		Last Modified: Sat, 02 Dec 2023 05:35:05 GMT  
		Size: 102.7 MB (102705543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbfa2ce417ae2a072f6f29b1e844390e6d9b5393778ab15be9c527becc70101`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7190a5e14d3e9d2629d582e66b149d4f59cef99a492b0724d24aeb70bbef7f01`  
		Last Modified: Sat, 02 Dec 2023 05:34:58 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34487c9ee277d9aca50f43642a87a4c62944214de3c137440c7fdd898ee68fb7`  
		Last Modified: Sat, 02 Dec 2023 10:48:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177847f4c9b0e7c56e31b57603d538db36b2dd8a591989cbfedb2755e9a3767a`  
		Last Modified: Wed, 13 Dec 2023 02:28:04 GMT  
		Size: 16.7 MB (16721081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c314abb53dc0b8a3567972ab762189d8c39b3b27a0d7bb51d16abaf9097b9f38`  
		Last Modified: Wed, 13 Dec 2023 02:28:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd2fbe787e03356684ed05713f1b902b7349a5662778c164442886925d57d8`  
		Last Modified: Wed, 13 Dec 2023 03:06:46 GMT  
		Size: 234.8 MB (234774375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d0e5410b941c5d87d34bb33c4001d7090812bd4dd35d34aeda97a0c004efd`  
		Last Modified: Wed, 13 Dec 2023 03:06:35 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8875427bb81d31fb6350053daf929e49b7b5bddcfb8f849553bb862d26a2e0`  
		Last Modified: Wed, 13 Dec 2023 03:06:59 GMT  
		Size: 13.6 MB (13600315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc12737831c1ef7e44c0c46cb11197fc953e0c5268264671d55ab3748619764`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342b64ed7620e9b42494093f48e23c935f04a2c7800e2ac063118bd90580d167`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d55dff1a0361827e2edef6886d87cd71a9c76adeda1282196952d869bddb7d`  
		Last Modified: Wed, 13 Dec 2023 03:06:57 GMT  
		Size: 973.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:3.12.11-postgres` - linux; ppc64le

```console
$ docker pull geonetwork@sha256:9db06fcf9ca87aba4305064c2458c0f9f3194d1d0ecfc08dc9da0a27def57ee7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.4 MB (411412373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231550a32a8924e94a329e0a9046129366f8a28e89eeceafe87c9cf3ffe81004`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:06:06 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 06:06:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 06:06:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 06:06:37 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:06:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 06:06:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 06:06:51 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 06:06:52 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 06:06:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 10:25:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 02 Dec 2023 10:25:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 10:25:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 02 Dec 2023 10:25:40 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 10:25:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:25:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 02 Dec 2023 10:41:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_MAJOR=8
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_VERSION=8.5.96
# Sat, 02 Dec 2023 10:41:10 GMT
ENV TOMCAT_SHA512=dc80b2649f2ad7f8baa6c925ef1d0bad71e27f5557dc46e313f45b8044dba05791a60062117d5257c28955f8405eded70e451ee2e0d9671c8aecd21977e0bec9
# Sat, 02 Dec 2023 10:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 02 Dec 2023 10:42:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 02 Dec 2023 10:42:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 10:42:35 GMT
ENTRYPOINT []
# Sat, 02 Dec 2023 10:42:35 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:26:37 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 11:26:37 GMT
ENV DATA_DIR=/usr/local/tomcat/webapps/geonetwork/WEB-INF/data
# Sat, 02 Dec 2023 11:26:37 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true -server -Xms512m -Xmx2024m -XX:NewSize=512m -XX:MaxNewSize=1024m -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_VERSION=3.12.11
# Sat, 02 Dec 2023 11:26:38 GMT
ENV GN_DOWNLOAD_MD5=2ece7076f05068e7a5270af03e32d632
# Sat, 02 Dec 2023 11:26:38 GMT
WORKDIR /usr/local/tomcat/webapps
# Sat, 02 Dec 2023 11:27:43 GMT
RUN apt-get update &&      apt-get install -y --no-install-recommends           unzip           curl &&     rm -rf /var/lib/apt/lists/* &&      curl -fSL -o $GN_FILE      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *${GN_FILE}" | md5sum -c &&      mkdir -p geonetwork &&      unzip -e $GN_FILE -d geonetwork &&      rm $GN_FILE
# Sat, 02 Dec 2023 11:27:49 GMT
COPY file:0804862fd42c05f06dfa65cb1e5dad9a956d8ac6a3ddd4d962847ba159f5cfe6 in /entrypoint.sh 
# Sat, 02 Dec 2023 11:27:50 GMT
WORKDIR /usr/local/tomcat
# Sat, 02 Dec 2023 11:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:27:51 GMT
CMD ["catalina.sh" "run"]
# Sat, 02 Dec 2023 11:28:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends postgresql-client &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 11:28:20 GMT
RUN sed -i -e 's#<import resource="../config-db/${geonetwork.db.type:h2}.xml"/>#<!--<import resource="../config-db/${geonetwork.db.type:h2}.xml"/-->#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml" && sed -i -e 's#<!--<import resource="../config-db/postgres.xml"/>-->#<import resource="../config-db/postgres.xml"/>#g' "${CATALINA_HOME}/webapps/geonetwork/WEB-INF/config-node/srv.xml"
# Sat, 02 Dec 2023 11:28:20 GMT
COPY file:83f69d2041e5fb378033b0db57e096c81ba0725102ab4da4f089685e748fcce3 in /usr/local/tomcat/webapps/geonetwork/WEB-INF/config-db/jdbc.properties 
# Sat, 02 Dec 2023 11:28:21 GMT
COPY file:c88411abba7ad9b7bb75019f08755dbfa163d2fc7fdd80676bf9350c4c56a19c in /entrypoint.sh 
# Sat, 02 Dec 2023 11:28:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 11:28:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8747a30614d194a60f1319fa2df5f984832ca89eb81acd4cb9a79921a3e29ee`  
		Last Modified: Sat, 02 Dec 2023 06:15:19 GMT  
		Size: 13.8 MB (13767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c19f99f6121dd20c43818a2074286ac3cd0a22717e6422bbd9906672d046eb`  
		Last Modified: Sat, 02 Dec 2023 06:15:26 GMT  
		Size: 101.1 MB (101068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796d159536564bd1bfdfc4bef9a60cfab9fc221a46f2b394fe279a76bd29f594`  
		Last Modified: Sat, 02 Dec 2023 06:15:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746424f05d58d8babd3b01ef35ebf619309db0dcecbc50d59f6228b9802b276b`  
		Last Modified: Sat, 02 Dec 2023 06:15:17 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412ae6901c0424f184ab0ea58f22bae66178343c613e0b6b2c22832e5467ae97`  
		Last Modified: Sat, 02 Dec 2023 10:54:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7268e9e471fc592cb0e2d2c70914c6a978ce0a4fcfe25f27e12921e045b5eb1`  
		Last Modified: Sat, 02 Dec 2023 10:59:02 GMT  
		Size: 11.9 MB (11902826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c83c246b991635e0dcec534581678e2d616ebe6a231bfd3e8642465de182e9`  
		Last Modified: Sat, 02 Dec 2023 10:59:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234830d9cb55a7c93a11ea60359c75c54f0e46a37a2c0927c66276b212d083b`  
		Last Modified: Sat, 02 Dec 2023 11:28:48 GMT  
		Size: 234.8 MB (234814373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71b89e91c60fef5d2f572846d938b75f573d16d3864e1740376e8fa926924b7`  
		Last Modified: Sat, 02 Dec 2023 11:28:33 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284724368be3e305ebd028f7302b24eaf424ae4e40fe163deceaf249dcc129c0`  
		Last Modified: Sat, 02 Dec 2023 11:29:04 GMT  
		Size: 14.2 MB (14191549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723ce2467d25e6aafcc85096e3e66b16dc0c68698b4fcc099346c4132cabb9d0`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7eedc2e35e020336f212e7af54e4a3f92626d1f1d2dee784360e75de85c36a`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eaf4c970558800ce1acbf0c774077201b0bfd0135b6b71e518027cde2672b7`  
		Last Modified: Sat, 02 Dec 2023 11:29:00 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4`

```console
$ docker pull geonetwork@sha256:f53c9815e184de2cda75a4bb4f575a2ff6e8d0fe15b6eb325dee5e860a900642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4` - linux; amd64

```console
$ docker pull geonetwork@sha256:6e0d3336e36f2adf99d8fe10181704bb76425549679a7f4f10ff415fc1a99d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.5 MB (471478021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c34a3dd7c79263ab171ac380f1d38b4eeff56a6edcbd7c71a1c6ef095256f4`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:59:10 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 01:59:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 01:59:20 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 01:59:21 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:59:21 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 01:59:21 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 07:11:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:12:14 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:12:14 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:12:14 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:12:14 GMT
USER jetty
# Sat, 02 Dec 2023 07:12:14 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:12:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:12:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:48 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:17:48 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:17:48 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:17:48 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:17:48 GMT
USER root
# Sat, 02 Dec 2023 13:17:53 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:17:53 GMT
USER jetty
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:18:14 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:18:16 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:18:16 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:18:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:18:17 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1402e25e07f840200989539b503bff8dd9c724aa7562877b2e7a0329564f1655`  
		Last Modified: Sat, 02 Dec 2023 02:04:44 GMT  
		Size: 145.3 MB (145275514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76a71f6791d66c0c053227b520b0f5e4480a5a82b5edbfc588d34eb5aa0e48`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f638494ca02b5ee71a2b33c337be4c779c8ef8325ff72f41f848dac9676a4`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9221bfc05e363eefcb21b87db27036e9cecf328b696c0ad5777245b91d78f90a`  
		Last Modified: Sat, 02 Dec 2023 07:21:01 GMT  
		Size: 10.3 MB (10268985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca794864cb51a37e80a0cab6ded9375da22943f49ce461bf4917998ab13c19`  
		Last Modified: Sat, 02 Dec 2023 07:21:00 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69798eed4b2e26147bb0c654640526e4024a5b192bda020a61b04eb6a620a6a0`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 482.7 KB (482709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910fefc34e3ee69e47b29e63746a919d9fbdf36256bb0e38eea479ff75b63347`  
		Last Modified: Sat, 02 Dec 2023 13:19:50 GMT  
		Size: 269.9 MB (269942768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356f61460a9e552c9dc143e9f37e371e9fb2fd4556526a93ef8a8762c609cf3`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7652942bb8b863271074d80513ecd99dfa3fd54fb120aba4e75ffdb62e4ea`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ecdac91a0a10939b75b7b85cb23847d016f9d230e65baa20c860588f889812`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:fe3cc705428e7893f524d2bd0fa008b54db5cbe3a49bfc4e0a17ddbbf279f767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75378f49154918fc5fe93cc1cc4b5bb61b50e5bc405b74aa6e7ca277cc2b17c7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 05:31:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 05:31:44 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:44 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:44 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 05:31:44 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:31:33 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:31:34 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:31:34 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:31:34 GMT
USER jetty
# Sat, 02 Dec 2023 09:31:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:31:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:31:34 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:38 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:53:38 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:53:39 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:53:39 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:53:39 GMT
USER root
# Sat, 02 Dec 2023 13:53:45 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:53:45 GMT
USER jetty
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:54:07 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:54:10 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:54:10 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:54:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:54:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073df27863e9816bf1fc5bc57fe02f5992b770de2e9267d1db025d767caa46d`  
		Last Modified: Sat, 02 Dec 2023 05:35:49 GMT  
		Size: 142.0 MB (142001755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b79bd989c382d3efa8d4e35afe2659b735726f501117b01a3f0acc6bfe2e6b`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb19c297ba820a5a4aa49c3c2678999bca146f8a5b6dce7936ab94be4e0c91`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc89707806f97e96efc3ec99e49b5a776e0460e523d59afbfd5433fccf9b4b4`  
		Last Modified: Sat, 02 Dec 2023 09:38:02 GMT  
		Size: 10.3 MB (10268843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8895a8d83dc4261f156f29f00f19457dad0388471949f592ee68f24ec1fabb`  
		Last Modified: Sat, 02 Dec 2023 09:38:01 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14ffa9c486ff287e984f7e9556d2434eacabbb16060d25c54fb805a0239e25`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 480.6 KB (480638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f4eac3446c2bb9df12eea995ca475b9441a60810672bae6459cbb7d8cd2dc`  
		Last Modified: Sat, 02 Dec 2023 13:55:37 GMT  
		Size: 269.9 MB (269942717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3779863a98a5816cfb985e1b62d178a65639e45d7c4e297354aae600aa057`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f029606c69795dcd3b37e9b3ea47ad7a2ef1f3890529ca779242ba0ce41ebfec`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e34a6b6a845a57e26deaa46d5a16aab7401a46f88da0672d1a112cfdfc99d8`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.2`

```console
$ docker pull geonetwork@sha256:94115ae5c76b982fe0e14be76f5c2062d8d6d355e69f9c76bd31a3225f223fc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.2` - linux; amd64

```console
$ docker pull geonetwork@sha256:14cbd1a60ab4cb9ce93db6c2ebe8bbaa744c587f8e3568b7ace0d79eb8efaf02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.9 MB (458885983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2adab22a634aba458c6a314e953e408399122c86a0630a5364a3d43fed60ec9f`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:57:57 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:03 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:03 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:03 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:10:37 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:10:37 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:10:37 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:10:38 GMT
USER jetty
# Sat, 02 Dec 2023 07:10:38 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:10:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:10:38 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:13:24 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:13:24 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 02 Dec 2023 13:13:24 GMT
USER root
# Sat, 02 Dec 2023 13:13:32 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 02 Dec 2023 13:13:32 GMT
USER jetty
# Sat, 02 Dec 2023 13:13:32 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:13:33 GMT
ENV GN_VERSION=4.2.7
# Sat, 02 Dec 2023 13:13:33 GMT
ENV GN_DOWNLOAD_MD5=0254ada0304b3cc09978405ba86cac8d
# Sat, 02 Dec 2023 13:17:43 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:17:44 GMT
COPY file:ee50548f90174fcbec925e62c4a2db15e8eb83e581b0f78e369d30fd096dcd23 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:17:44 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:17:44 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:44 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d86b1034015687b97b9d97585d23b47fed7a9a89809993fcd9566a699bc46a`  
		Last Modified: Sat, 02 Dec 2023 02:03:32 GMT  
		Size: 103.6 MB (103597494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052c2083d35267d7e4960f75b3278112b6ad459d7dfaf496c0792ff4071e09f0`  
		Last Modified: Sat, 02 Dec 2023 02:03:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78e4548434efaa554eeca11e58727767550efc9a420448712dcac7b9d9db3dc`  
		Last Modified: Sat, 02 Dec 2023 02:03:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9330eca0a19090fb8e4fe7c8da3b033a2cc2311d05377f3908d2c2db37a97c4`  
		Last Modified: Sat, 02 Dec 2023 07:20:10 GMT  
		Size: 10.3 MB (10267422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f6aaa7169af57dfa14dd6776605af156d5a324b5227c7b35e07ce714d180e8`  
		Last Modified: Sat, 02 Dec 2023 07:20:09 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9f74c4ff171670837f7886146c1f98007700a4f1cbd36bdff4d6d4bf246843`  
		Last Modified: Sat, 02 Dec 2023 13:19:11 GMT  
		Size: 482.8 KB (482767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d02e998264aba9b86f6790d26595d0b522d47770009f064e8287f99456d4cf`  
		Last Modified: Sat, 02 Dec 2023 13:19:27 GMT  
		Size: 299.0 MB (299030618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb28b33111035293758a98ebc822235bbea77ea8f66482738d63084a0e1b893`  
		Last Modified: Sat, 02 Dec 2023 13:19:11 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.2` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:db4c903ed06c0b6d8bb00110ebc2943c720439b51303c8041fae6b2b04c41acf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456461501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae6323291fbfb4b75f6e909a07225401f47ab75a8eae95a2b7cb0f4a6d6718a8`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:30:41 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:30:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:30:48 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:30:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:30:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:30:31 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:30:31 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:30:31 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:30:31 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:30:49 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:30:50 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:30:50 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:30:50 GMT
USER jetty
# Sat, 02 Dec 2023 09:30:50 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:30:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:30:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:49:16 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:49:16 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 02 Dec 2023 13:49:16 GMT
USER root
# Sat, 02 Dec 2023 13:49:21 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 02 Dec 2023 13:49:21 GMT
USER jetty
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_VERSION=4.2.7
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_DOWNLOAD_MD5=0254ada0304b3cc09978405ba86cac8d
# Sat, 02 Dec 2023 13:53:19 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:53:22 GMT
COPY file:ee50548f90174fcbec925e62c4a2db15e8eb83e581b0f78e369d30fd096dcd23 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:53:22 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:53:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:22 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552ea4c77814dcce1009cd9ac5ba2ed01f9a105bb53c8f3eeb2612fef2e2e1b0`  
		Last Modified: Sat, 02 Dec 2023 05:34:48 GMT  
		Size: 102.7 MB (102707028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5edb978b3ff186ea9e0512581c2ca20f032ca47fc0c20650d9dec6ef36cfc9`  
		Last Modified: Sat, 02 Dec 2023 05:34:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648e51319be7039b18137ff4145fed67f06a3bd172a3532e5d7e7e4f28acac57`  
		Last Modified: Sat, 02 Dec 2023 05:34:41 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d2b43cba8ef96f5945f249cab0e2e2f369255c663ef0899c946a1ac0c959a`  
		Last Modified: Sat, 02 Dec 2023 09:37:18 GMT  
		Size: 10.3 MB (10267313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010089565d95ea1787fe81adeeeaaef8e6e2cb3a3f7c81a398be7ad7cd07533d`  
		Last Modified: Sat, 02 Dec 2023 09:37:17 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9107f594e0fe6c32a938de32c1d09321ff6143a2a9d9cf37d5dedb9b0b5685ce`  
		Last Modified: Sat, 02 Dec 2023 13:55:04 GMT  
		Size: 480.8 KB (480764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bc7490da5c843685ff2c219453529b0bcb5e0ee581090e887a08cba6a89fd`  
		Last Modified: Sat, 02 Dec 2023 13:55:17 GMT  
		Size: 299.0 MB (299030620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cc658b797541c21498d67f619adba934e0c62aaab452816ea26ecc0a3a2c41`  
		Last Modified: Sat, 02 Dec 2023 13:55:03 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.2.7`

```console
$ docker pull geonetwork@sha256:94115ae5c76b982fe0e14be76f5c2062d8d6d355e69f9c76bd31a3225f223fc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.2.7` - linux; amd64

```console
$ docker pull geonetwork@sha256:14cbd1a60ab4cb9ce93db6c2ebe8bbaa744c587f8e3568b7ace0d79eb8efaf02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.9 MB (458885983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2adab22a634aba458c6a314e953e408399122c86a0630a5364a3d43fed60ec9f`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:57:57 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 01:58:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 01:58:03 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 01:58:03 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:58:03 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:10:16 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:10:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:10:37 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:10:37 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:10:37 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:10:38 GMT
USER jetty
# Sat, 02 Dec 2023 07:10:38 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:10:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:10:38 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:13:24 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:13:24 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 02 Dec 2023 13:13:24 GMT
USER root
# Sat, 02 Dec 2023 13:13:32 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 02 Dec 2023 13:13:32 GMT
USER jetty
# Sat, 02 Dec 2023 13:13:32 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:13:33 GMT
ENV GN_VERSION=4.2.7
# Sat, 02 Dec 2023 13:13:33 GMT
ENV GN_DOWNLOAD_MD5=0254ada0304b3cc09978405ba86cac8d
# Sat, 02 Dec 2023 13:17:43 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:17:44 GMT
COPY file:ee50548f90174fcbec925e62c4a2db15e8eb83e581b0f78e369d30fd096dcd23 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:17:44 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:17:44 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:44 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d86b1034015687b97b9d97585d23b47fed7a9a89809993fcd9566a699bc46a`  
		Last Modified: Sat, 02 Dec 2023 02:03:32 GMT  
		Size: 103.6 MB (103597494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052c2083d35267d7e4960f75b3278112b6ad459d7dfaf496c0792ff4071e09f0`  
		Last Modified: Sat, 02 Dec 2023 02:03:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78e4548434efaa554eeca11e58727767550efc9a420448712dcac7b9d9db3dc`  
		Last Modified: Sat, 02 Dec 2023 02:03:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9330eca0a19090fb8e4fe7c8da3b033a2cc2311d05377f3908d2c2db37a97c4`  
		Last Modified: Sat, 02 Dec 2023 07:20:10 GMT  
		Size: 10.3 MB (10267422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f6aaa7169af57dfa14dd6776605af156d5a324b5227c7b35e07ce714d180e8`  
		Last Modified: Sat, 02 Dec 2023 07:20:09 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9f74c4ff171670837f7886146c1f98007700a4f1cbd36bdff4d6d4bf246843`  
		Last Modified: Sat, 02 Dec 2023 13:19:11 GMT  
		Size: 482.8 KB (482767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d02e998264aba9b86f6790d26595d0b522d47770009f064e8287f99456d4cf`  
		Last Modified: Sat, 02 Dec 2023 13:19:27 GMT  
		Size: 299.0 MB (299030618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb28b33111035293758a98ebc822235bbea77ea8f66482738d63084a0e1b893`  
		Last Modified: Sat, 02 Dec 2023 13:19:11 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.2.7` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:db4c903ed06c0b6d8bb00110ebc2943c720439b51303c8041fae6b2b04c41acf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.5 MB (456461501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae6323291fbfb4b75f6e909a07225401f47ab75a8eae95a2b7cb0f4a6d6718a8`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:30:41 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Sat, 02 Dec 2023 05:30:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='70636c2fa4927913e9e869d471607a99d3a521c1fa3f3687b889c2acba67c493';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u392b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='15d091e22aa0cad12a241acff8c1634e7228b9740f8d19634250aa6fe0c19a33';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u392b08.tar.gz';          ;;        armhf|arm)          ESUM='9e574cff0b8dba29930e38eeec4cb4350a77a56a27d03fa316fa6b2383eeef9d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_arm_linux_hotspot_8u392b08.tar.gz';          apt-get update;          DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1;          rm -rf /var/lib/apt/lists/*;          ;;        ppc64el|powerpc:common64)          ESUM='9d9813d2840360ffdbc449c45e71124e8170c31a3b6cce9151fbb31352064406';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u392b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Dec 2023 05:30:48 GMT
RUN set -eux;     echo "Verifying install ...";     echo "javac -version"; javac -version;     echo "java -version"; java -version;     echo "Complete."
# Sat, 02 Dec 2023 05:30:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:30:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:30:30 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:30:31 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:30:31 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:30:31 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:30:31 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:30:49 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:30:50 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:30:50 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:30:50 GMT
USER jetty
# Sat, 02 Dec 2023 09:30:50 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:30:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:30:50 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:49:16 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:49:16 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Sat, 02 Dec 2023 13:49:16 GMT
USER root
# Sat, 02 Dec 2023 13:49:21 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Sat, 02 Dec 2023 13:49:21 GMT
USER jetty
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_VERSION=4.2.7
# Sat, 02 Dec 2023 13:49:21 GMT
ENV GN_DOWNLOAD_MD5=0254ada0304b3cc09978405ba86cac8d
# Sat, 02 Dec 2023 13:53:19 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:53:22 GMT
COPY file:ee50548f90174fcbec925e62c4a2db15e8eb83e581b0f78e369d30fd096dcd23 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:53:22 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:53:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:22 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552ea4c77814dcce1009cd9ac5ba2ed01f9a105bb53c8f3eeb2612fef2e2e1b0`  
		Last Modified: Sat, 02 Dec 2023 05:34:48 GMT  
		Size: 102.7 MB (102707028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5edb978b3ff186ea9e0512581c2ca20f032ca47fc0c20650d9dec6ef36cfc9`  
		Last Modified: Sat, 02 Dec 2023 05:34:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648e51319be7039b18137ff4145fed67f06a3bd172a3532e5d7e7e4f28acac57`  
		Last Modified: Sat, 02 Dec 2023 05:34:41 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578d2b43cba8ef96f5945f249cab0e2e2f369255c663ef0899c946a1ac0c959a`  
		Last Modified: Sat, 02 Dec 2023 09:37:18 GMT  
		Size: 10.3 MB (10267313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010089565d95ea1787fe81adeeeaaef8e6e2cb3a3f7c81a398be7ad7cd07533d`  
		Last Modified: Sat, 02 Dec 2023 09:37:17 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9107f594e0fe6c32a938de32c1d09321ff6143a2a9d9cf37d5dedb9b0b5685ce`  
		Last Modified: Sat, 02 Dec 2023 13:55:04 GMT  
		Size: 480.8 KB (480764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50bc7490da5c843685ff2c219453529b0bcb5e0ee581090e887a08cba6a89fd`  
		Last Modified: Sat, 02 Dec 2023 13:55:17 GMT  
		Size: 299.0 MB (299030620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cc658b797541c21498d67f619adba934e0c62aaab452816ea26ecc0a3a2c41`  
		Last Modified: Sat, 02 Dec 2023 13:55:03 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.4`

```console
$ docker pull geonetwork@sha256:f53c9815e184de2cda75a4bb4f575a2ff6e8d0fe15b6eb325dee5e860a900642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.4` - linux; amd64

```console
$ docker pull geonetwork@sha256:6e0d3336e36f2adf99d8fe10181704bb76425549679a7f4f10ff415fc1a99d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.5 MB (471478021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c34a3dd7c79263ab171ac380f1d38b4eeff56a6edcbd7c71a1c6ef095256f4`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:59:10 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 01:59:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 01:59:20 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 01:59:21 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:59:21 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 01:59:21 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 07:11:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:12:14 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:12:14 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:12:14 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:12:14 GMT
USER jetty
# Sat, 02 Dec 2023 07:12:14 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:12:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:12:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:48 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:17:48 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:17:48 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:17:48 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:17:48 GMT
USER root
# Sat, 02 Dec 2023 13:17:53 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:17:53 GMT
USER jetty
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:18:14 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:18:16 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:18:16 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:18:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:18:17 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1402e25e07f840200989539b503bff8dd9c724aa7562877b2e7a0329564f1655`  
		Last Modified: Sat, 02 Dec 2023 02:04:44 GMT  
		Size: 145.3 MB (145275514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76a71f6791d66c0c053227b520b0f5e4480a5a82b5edbfc588d34eb5aa0e48`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f638494ca02b5ee71a2b33c337be4c779c8ef8325ff72f41f848dac9676a4`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9221bfc05e363eefcb21b87db27036e9cecf328b696c0ad5777245b91d78f90a`  
		Last Modified: Sat, 02 Dec 2023 07:21:01 GMT  
		Size: 10.3 MB (10268985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca794864cb51a37e80a0cab6ded9375da22943f49ce461bf4917998ab13c19`  
		Last Modified: Sat, 02 Dec 2023 07:21:00 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69798eed4b2e26147bb0c654640526e4024a5b192bda020a61b04eb6a620a6a0`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 482.7 KB (482709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910fefc34e3ee69e47b29e63746a919d9fbdf36256bb0e38eea479ff75b63347`  
		Last Modified: Sat, 02 Dec 2023 13:19:50 GMT  
		Size: 269.9 MB (269942768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356f61460a9e552c9dc143e9f37e371e9fb2fd4556526a93ef8a8762c609cf3`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7652942bb8b863271074d80513ecd99dfa3fd54fb120aba4e75ffdb62e4ea`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ecdac91a0a10939b75b7b85cb23847d016f9d230e65baa20c860588f889812`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.4` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:fe3cc705428e7893f524d2bd0fa008b54db5cbe3a49bfc4e0a17ddbbf279f767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75378f49154918fc5fe93cc1cc4b5bb61b50e5bc405b74aa6e7ca277cc2b17c7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 05:31:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 05:31:44 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:44 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:44 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 05:31:44 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:31:33 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:31:34 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:31:34 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:31:34 GMT
USER jetty
# Sat, 02 Dec 2023 09:31:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:31:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:31:34 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:38 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:53:38 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:53:39 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:53:39 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:53:39 GMT
USER root
# Sat, 02 Dec 2023 13:53:45 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:53:45 GMT
USER jetty
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:54:07 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:54:10 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:54:10 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:54:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:54:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073df27863e9816bf1fc5bc57fe02f5992b770de2e9267d1db025d767caa46d`  
		Last Modified: Sat, 02 Dec 2023 05:35:49 GMT  
		Size: 142.0 MB (142001755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b79bd989c382d3efa8d4e35afe2659b735726f501117b01a3f0acc6bfe2e6b`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb19c297ba820a5a4aa49c3c2678999bca146f8a5b6dce7936ab94be4e0c91`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc89707806f97e96efc3ec99e49b5a776e0460e523d59afbfd5433fccf9b4b4`  
		Last Modified: Sat, 02 Dec 2023 09:38:02 GMT  
		Size: 10.3 MB (10268843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8895a8d83dc4261f156f29f00f19457dad0388471949f592ee68f24ec1fabb`  
		Last Modified: Sat, 02 Dec 2023 09:38:01 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14ffa9c486ff287e984f7e9556d2434eacabbb16060d25c54fb805a0239e25`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 480.6 KB (480638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f4eac3446c2bb9df12eea995ca475b9441a60810672bae6459cbb7d8cd2dc`  
		Last Modified: Sat, 02 Dec 2023 13:55:37 GMT  
		Size: 269.9 MB (269942717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3779863a98a5816cfb985e1b62d178a65639e45d7c4e297354aae600aa057`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f029606c69795dcd3b37e9b3ea47ad7a2ef1f3890529ca779242ba0ce41ebfec`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e34a6b6a845a57e26deaa46d5a16aab7401a46f88da0672d1a112cfdfc99d8`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:4.4.1`

```console
$ docker pull geonetwork@sha256:f53c9815e184de2cda75a4bb4f575a2ff6e8d0fe15b6eb325dee5e860a900642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:4.4.1` - linux; amd64

```console
$ docker pull geonetwork@sha256:6e0d3336e36f2adf99d8fe10181704bb76425549679a7f4f10ff415fc1a99d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.5 MB (471478021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c34a3dd7c79263ab171ac380f1d38b4eeff56a6edcbd7c71a1c6ef095256f4`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:59:10 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 01:59:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 01:59:20 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 01:59:21 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:59:21 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 01:59:21 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 07:11:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:12:14 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:12:14 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:12:14 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:12:14 GMT
USER jetty
# Sat, 02 Dec 2023 07:12:14 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:12:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:12:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:48 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:17:48 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:17:48 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:17:48 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:17:48 GMT
USER root
# Sat, 02 Dec 2023 13:17:53 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:17:53 GMT
USER jetty
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:18:14 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:18:16 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:18:16 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:18:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:18:17 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1402e25e07f840200989539b503bff8dd9c724aa7562877b2e7a0329564f1655`  
		Last Modified: Sat, 02 Dec 2023 02:04:44 GMT  
		Size: 145.3 MB (145275514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76a71f6791d66c0c053227b520b0f5e4480a5a82b5edbfc588d34eb5aa0e48`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f638494ca02b5ee71a2b33c337be4c779c8ef8325ff72f41f848dac9676a4`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9221bfc05e363eefcb21b87db27036e9cecf328b696c0ad5777245b91d78f90a`  
		Last Modified: Sat, 02 Dec 2023 07:21:01 GMT  
		Size: 10.3 MB (10268985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca794864cb51a37e80a0cab6ded9375da22943f49ce461bf4917998ab13c19`  
		Last Modified: Sat, 02 Dec 2023 07:21:00 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69798eed4b2e26147bb0c654640526e4024a5b192bda020a61b04eb6a620a6a0`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 482.7 KB (482709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910fefc34e3ee69e47b29e63746a919d9fbdf36256bb0e38eea479ff75b63347`  
		Last Modified: Sat, 02 Dec 2023 13:19:50 GMT  
		Size: 269.9 MB (269942768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356f61460a9e552c9dc143e9f37e371e9fb2fd4556526a93ef8a8762c609cf3`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7652942bb8b863271074d80513ecd99dfa3fd54fb120aba4e75ffdb62e4ea`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ecdac91a0a10939b75b7b85cb23847d016f9d230e65baa20c860588f889812`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:4.4.1` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:fe3cc705428e7893f524d2bd0fa008b54db5cbe3a49bfc4e0a17ddbbf279f767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75378f49154918fc5fe93cc1cc4b5bb61b50e5bc405b74aa6e7ca277cc2b17c7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 05:31:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 05:31:44 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:44 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:44 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 05:31:44 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:31:33 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:31:34 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:31:34 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:31:34 GMT
USER jetty
# Sat, 02 Dec 2023 09:31:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:31:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:31:34 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:38 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:53:38 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:53:39 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:53:39 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:53:39 GMT
USER root
# Sat, 02 Dec 2023 13:53:45 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:53:45 GMT
USER jetty
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:54:07 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:54:10 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:54:10 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:54:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:54:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073df27863e9816bf1fc5bc57fe02f5992b770de2e9267d1db025d767caa46d`  
		Last Modified: Sat, 02 Dec 2023 05:35:49 GMT  
		Size: 142.0 MB (142001755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b79bd989c382d3efa8d4e35afe2659b735726f501117b01a3f0acc6bfe2e6b`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb19c297ba820a5a4aa49c3c2678999bca146f8a5b6dce7936ab94be4e0c91`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc89707806f97e96efc3ec99e49b5a776e0460e523d59afbfd5433fccf9b4b4`  
		Last Modified: Sat, 02 Dec 2023 09:38:02 GMT  
		Size: 10.3 MB (10268843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8895a8d83dc4261f156f29f00f19457dad0388471949f592ee68f24ec1fabb`  
		Last Modified: Sat, 02 Dec 2023 09:38:01 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14ffa9c486ff287e984f7e9556d2434eacabbb16060d25c54fb805a0239e25`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 480.6 KB (480638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f4eac3446c2bb9df12eea995ca475b9441a60810672bae6459cbb7d8cd2dc`  
		Last Modified: Sat, 02 Dec 2023 13:55:37 GMT  
		Size: 269.9 MB (269942717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3779863a98a5816cfb985e1b62d178a65639e45d7c4e297354aae600aa057`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f029606c69795dcd3b37e9b3ea47ad7a2ef1f3890529ca779242ba0ce41ebfec`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e34a6b6a845a57e26deaa46d5a16aab7401a46f88da0672d1a112cfdfc99d8`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `geonetwork:latest`

```console
$ docker pull geonetwork@sha256:f53c9815e184de2cda75a4bb4f575a2ff6e8d0fe15b6eb325dee5e860a900642
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:latest` - linux; amd64

```console
$ docker pull geonetwork@sha256:6e0d3336e36f2adf99d8fe10181704bb76425549679a7f4f10ff415fc1a99d16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.5 MB (471478021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6c34a3dd7c79263ab171ac380f1d38b4eeff56a6edcbd7c71a1c6ef095256f4`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 01:57:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 01:57:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 01:57:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 01:57:57 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 01:59:10 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 01:59:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 01:59:20 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 01:59:21 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 01:59:21 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 01:59:21 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 07:11:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 07:11:14 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 07:11:14 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 07:12:14 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 07:12:14 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 07:12:14 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 07:12:14 GMT
USER jetty
# Sat, 02 Dec 2023 07:12:14 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 07:12:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:12:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:17:48 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:17:48 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:17:48 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:17:48 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:17:48 GMT
USER root
# Sat, 02 Dec 2023 13:17:53 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:17:53 GMT
USER jetty
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:17:53 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:18:14 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:18:15 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:18:16 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:18:16 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:18:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:18:17 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3ed95e21625a2f60f42187379932a7ccaed17dc9647e941ced64e1124b3342`  
		Last Modified: Sat, 02 Dec 2023 02:03:26 GMT  
		Size: 16.9 MB (16920158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1402e25e07f840200989539b503bff8dd9c724aa7562877b2e7a0329564f1655`  
		Last Modified: Sat, 02 Dec 2023 02:04:44 GMT  
		Size: 145.3 MB (145275514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e76a71f6791d66c0c053227b520b0f5e4480a5a82b5edbfc588d34eb5aa0e48`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38f638494ca02b5ee71a2b33c337be4c779c8ef8325ff72f41f848dac9676a4`  
		Last Modified: Sat, 02 Dec 2023 02:04:32 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9221bfc05e363eefcb21b87db27036e9cecf328b696c0ad5777245b91d78f90a`  
		Last Modified: Sat, 02 Dec 2023 07:21:01 GMT  
		Size: 10.3 MB (10268985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ca794864cb51a37e80a0cab6ded9375da22943f49ce461bf4917998ab13c19`  
		Last Modified: Sat, 02 Dec 2023 07:21:00 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69798eed4b2e26147bb0c654640526e4024a5b192bda020a61b04eb6a620a6a0`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 482.7 KB (482709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910fefc34e3ee69e47b29e63746a919d9fbdf36256bb0e38eea479ff75b63347`  
		Last Modified: Sat, 02 Dec 2023 13:19:50 GMT  
		Size: 269.9 MB (269942768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5356f61460a9e552c9dc143e9f37e371e9fb2fd4556526a93ef8a8762c609cf3`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7652942bb8b863271074d80513ecd99dfa3fd54fb120aba4e75ffdb62e4ea`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ecdac91a0a10939b75b7b85cb23847d016f9d230e65baa20c860588f889812`  
		Last Modified: Sat, 02 Dec 2023 13:19:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:latest` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:fe3cc705428e7893f524d2bd0fa008b54db5cbe3a49bfc4e0a17ddbbf279f767
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.7 MB (466670099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75378f49154918fc5fe93cc1cc4b5bb61b50e5bc405b74aa6e7ca277cc2b17c7`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:30:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 05:30:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:30:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:30:41 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:31:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Sat, 02 Dec 2023 05:31:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8c3146035b99c55ab26a2982f4b9abd2bf600582361cf9c732539f713d271faf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='60ea98daa09834fdd3162ca91ddc8d92a155ab3121204f6f643176ee0c2d0d5e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='a64b005b84b173e294078fec34660ed3429d8c60726a5fb5c140e13b9e0c79fa';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='262ff98d6d88a7c7cc522cb4ec4129491a0eb04f5b17dcca0da57cfcdcf3830d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bc67f79fb82c4131d9dcea32649c540a16aa380a9726306b9a67c5ec9690c492';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Dec 2023 05:31:44 GMT
RUN set -eux;     echo "Verifying install ...";     fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java;     echo "javac --version"; javac --version;     echo "java --version"; java --version;     echo "Complete."
# Sat, 02 Dec 2023 05:31:44 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Dec 2023 05:31:44 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Sat, 02 Dec 2023 05:31:44 GMT
CMD ["jshell"]
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_VERSION=9.4.53.v20231009
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV TMPDIR=/tmp/jetty
# Sat, 02 Dec 2023 09:31:13 GMT
ENV PATH=/usr/local/jetty/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.53.v20231009/jetty-home-9.4.53.v20231009.tar.gz
# Sat, 02 Dec 2023 09:31:13 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3
# Sat, 02 Dec 2023 09:31:33 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	case "$JETTY_VERSION" in 		"12."*) START_MODULES="server,http,ext,resources" ;; 		*) START_MODULES="server,http,deploy,ext,resources,jsp,jstl,websocket" ;; 	esac ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="$START_MODULES" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sat, 02 Dec 2023 09:31:34 GMT
WORKDIR /var/lib/jetty
# Sat, 02 Dec 2023 09:31:34 GMT
COPY multi:6bf6ffc2c0ff756d51254f4ec987e84575c16c895c328c42a63bde92f8d5278a in / 
# Sat, 02 Dec 2023 09:31:34 GMT
USER jetty
# Sat, 02 Dec 2023 09:31:34 GMT
EXPOSE 8080
# Sat, 02 Dec 2023 09:31:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 09:31:34 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:53:38 GMT
ENV DATA_DIR=/catalogue-data
# Sat, 02 Dec 2023 13:53:38 GMT
ENV WEBAPP_CONTEXT_PATH=/geonetwork
# Sat, 02 Dec 2023 13:53:39 GMT
ENV GN_CONFIG_PROPERTIES=-Dgeonetwork.dir=/catalogue-data         -Dgeonetwork.formatter.dir=/catalogue-data/data/formatter         -Dgeonetwork.schema.dir=/opt/geonetwork/WEB-INF/data/config/schema_plugins         -Dgeonetwork.indexConfig.dir=/opt/geonetwork/WEB-INF/data/config/index
# Sat, 02 Dec 2023 13:53:39 GMT
ENV JAVA_OPTS=-Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC
# Sat, 02 Dec 2023 13:53:39 GMT
USER root
# Sat, 02 Dec 2023 13:53:45 GMT
RUN apt-get -y update &&     apt-get -y install --no-install-recommends         curl         unzip &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p ${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /opt/geonetwork &&     chown -R jetty:jetty /opt/geonetwork
# Sat, 02 Dec 2023 13:53:45 GMT
USER jetty
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_FILE=geonetwork.war
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_VERSION=4.4.1
# Sat, 02 Dec 2023 13:53:45 GMT
ENV GN_DOWNLOAD_MD5=ff40fb2033e67b83f22246d52d04092e
# Sat, 02 Dec 2023 13:54:07 GMT
RUN cd /opt/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:996df24c69b17d351426a6c0c0dfb153f784c21af81ae4ec36afa187063e1eda in /usr/local/share/geonetwork/geonetwork_context_template.xml 
# Sat, 02 Dec 2023 13:54:09 GMT
COPY file:d79abcd242af427d06aee0b458cf9b6d258c1203248aa30f6246fc26f5727df3 in /geonetwork-entrypoint.sh 
# Sat, 02 Dec 2023 13:54:10 GMT
RUN java -jar /usr/local/jetty/start.jar --create-startd --add-module=http-forwarded
# Sat, 02 Dec 2023 13:54:10 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Sat, 02 Dec 2023 13:54:10 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Sat, 02 Dec 2023 13:54:10 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ec55d497e7d6fc44f37c9265653680043adfe45e40de6c9842409c66f59f76`  
		Last Modified: Sat, 02 Dec 2023 05:34:43 GMT  
		Size: 16.8 MB (16768418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0073df27863e9816bf1fc5bc57fe02f5992b770de2e9267d1db025d767caa46d`  
		Last Modified: Sat, 02 Dec 2023 05:35:49 GMT  
		Size: 142.0 MB (142001755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b79bd989c382d3efa8d4e35afe2659b735726f501117b01a3f0acc6bfe2e6b`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eb19c297ba820a5a4aa49c3c2678999bca146f8a5b6dce7936ab94be4e0c91`  
		Last Modified: Sat, 02 Dec 2023 05:35:41 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc89707806f97e96efc3ec99e49b5a776e0460e523d59afbfd5433fccf9b4b4`  
		Last Modified: Sat, 02 Dec 2023 09:38:02 GMT  
		Size: 10.3 MB (10268843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8895a8d83dc4261f156f29f00f19457dad0388471949f592ee68f24ec1fabb`  
		Last Modified: Sat, 02 Dec 2023 09:38:01 GMT  
		Size: 1.6 KB (1634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14ffa9c486ff287e984f7e9556d2434eacabbb16060d25c54fb805a0239e25`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 480.6 KB (480638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f4eac3446c2bb9df12eea995ca475b9441a60810672bae6459cbb7d8cd2dc`  
		Last Modified: Sat, 02 Dec 2023 13:55:37 GMT  
		Size: 269.9 MB (269942717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3779863a98a5816cfb985e1b62d178a65639e45d7c4e297354aae600aa057`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f029606c69795dcd3b37e9b3ea47ad7a2ef1f3890529ca779242ba0ce41ebfec`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 568.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e34a6b6a845a57e26deaa46d5a16aab7401a46f88da0672d1a112cfdfc99d8`  
		Last Modified: Sat, 02 Dec 2023 13:55:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
