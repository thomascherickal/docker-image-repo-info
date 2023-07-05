## `tomcat:8-jdk17-temurin-focal`

```console
$ docker pull tomcat@sha256:ef14caf0d984e8f2dc3724ef110ac2c6be31619b66d57783f6d92aa275d7372f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jdk17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:b61de682f9544de96ed708cd2f9f5412f44afce14dc0288ca4c0e95ab79bfca6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253184538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91dfc65e678caee871ca43fbc955b91dfd37634030eade566de9c3ec852e5f99`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:18:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:18:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:18:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:18:14 GMT
CMD ["jshell"]
# Fri, 16 Jun 2023 04:35:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 16 Jun 2023 04:35:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 04:35:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 16 Jun 2023 04:35:57 GMT
WORKDIR /usr/local/tomcat
# Fri, 16 Jun 2023 04:35:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 04:35:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 04:41:14 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 16 Jun 2023 04:41:14 GMT
ENV TOMCAT_MAJOR=8
# Fri, 16 Jun 2023 04:41:14 GMT
ENV TOMCAT_VERSION=8.5.90
# Fri, 16 Jun 2023 04:41:14 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Fri, 16 Jun 2023 04:41:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Fri, 16 Jun 2023 04:41:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 16 Jun 2023 04:41:49 GMT
EXPOSE 8080
# Fri, 16 Jun 2023 04:41:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf068c018154ad6aca69d7f48df2e3b365cdc9b1c644b1b5028cd5eb9bd6e6`  
		Last Modified: Fri, 16 Jun 2023 02:23:07 GMT  
		Size: 20.2 MB (20155613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d093beb2f5fb9c0536b0d235c91ff601ae8f0100da8f8401ca0b87e5e2730de4`  
		Last Modified: Fri, 16 Jun 2023 02:23:18 GMT  
		Size: 192.6 MB (192587830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bbba3d29536b69c7ed1ee0cd1c6f384e4a03fc8c2a9fe7b7874be7a95a600a`  
		Last Modified: Fri, 16 Jun 2023 02:23:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966e2a331d3fc64e7670a24b61d3ce597b6cf430eeb5858288ea5e065fdd863`  
		Last Modified: Fri, 16 Jun 2023 04:50:33 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e9b5c2460fa5b6c972799f728900c1712b2d2f0298091efd0feca47167c834`  
		Last Modified: Fri, 16 Jun 2023 04:54:23 GMT  
		Size: 11.9 MB (11860099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd1ae4d478c23794bba46df7350a1f0070590bc91a2dcb91ba1cb54ffc8db6`  
		Last Modified: Fri, 16 Jun 2023 04:54:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:233ab85f1b6de271c88c402fff7cbd83bdfd2ed8caaf6f84bf547fe092fc6413
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245512662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d8cff1e587dfb0aebaba69400cba8cb87bd87e556ff97d9a95435c2241fe9c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 05 Jun 2023 17:19:26 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:19:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:19:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:19:27 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:19:31 GMT
ADD file:114d6f55f8c1c4ec7f7d2ba3c803116a188eece1d1b6dbb3bb40c11082194234 in / 
# Mon, 05 Jun 2023 17:19:31 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:24:33 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 01:24:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 01:24:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 01:27:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:27:27 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 01:27:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 01:27:42 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 01:27:42 GMT
CMD ["jshell"]
# Fri, 16 Jun 2023 02:18:09 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 16 Jun 2023 02:18:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:18:09 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 16 Jun 2023 02:18:10 GMT
WORKDIR /usr/local/tomcat
# Fri, 16 Jun 2023 02:18:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 02:18:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 02:22:38 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 16 Jun 2023 02:22:38 GMT
ENV TOMCAT_MAJOR=8
# Fri, 16 Jun 2023 02:22:38 GMT
ENV TOMCAT_VERSION=8.5.90
# Fri, 16 Jun 2023 02:22:38 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Fri, 16 Jun 2023 02:23:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Fri, 16 Jun 2023 02:23:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 16 Jun 2023 02:23:10 GMT
EXPOSE 8080
# Fri, 16 Jun 2023 02:23:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2d97abfcf215d35e8a846b390350fea9f455676b41221360fe8782163a1c46bb`  
		Last Modified: Thu, 15 Jun 2023 03:47:54 GMT  
		Size: 24.6 MB (24589116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9067cc6505509e2b7bb16e7f0c09847b2c08d84d194afcfb81a01431688d9b`  
		Last Modified: Fri, 16 Jun 2023 01:31:24 GMT  
		Size: 19.5 MB (19538930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b239e758bbd4caeabeaca58525e3c301094cff402399da0ab3b370ea108f60f8`  
		Last Modified: Fri, 16 Jun 2023 01:31:36 GMT  
		Size: 189.6 MB (189596893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8e47de6fa8a3fc30e380234cd552227e35ff796e648073d11ce68ac5513d6`  
		Last Modified: Fri, 16 Jun 2023 01:31:21 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b22395a5c620cd5781b22f06b7a8a74d3d6af9dc064f6d96b767fb6b5f93cd`  
		Last Modified: Fri, 16 Jun 2023 02:31:14 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d03c5a9d54ae36ceaafae70b79831ee3f58a0b23d964b3291c355521ae4e6d`  
		Last Modified: Fri, 16 Jun 2023 02:34:49 GMT  
		Size: 11.8 MB (11787247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a8c36fa87ac4bbe00f6ff1a9cf90902197df8b8dd19e146f72373dadf26305`  
		Last Modified: Fri, 16 Jun 2023 02:34:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:61554795093b0a538b098c37e50b7689b99e1c07b27549ed50a4901ad980f2d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.3 MB (251333565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ae6ef873630a5b54965fa6d5dd25459ac4438e41abdf8f59e865893e7621796`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:11 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 15:34:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:34:24 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Tue, 04 Jul 2023 15:34:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 15:34:38 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 04 Jul 2023 15:34:38 GMT
CMD ["jshell"]
# Wed, 05 Jul 2023 02:58:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 02:58:46 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 02:58:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 02:58:46 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 02:58:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 02:58:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 03:05:58 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 05 Jul 2023 03:05:58 GMT
ENV TOMCAT_MAJOR=8
# Wed, 05 Jul 2023 03:05:58 GMT
ENV TOMCAT_VERSION=8.5.90
# Wed, 05 Jul 2023 03:05:58 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Wed, 05 Jul 2023 03:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 05 Jul 2023 03:06:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 05 Jul 2023 03:06:28 GMT
EXPOSE 8080
# Wed, 05 Jul 2023 03:06:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1684b62594f0c379e1487e5985d72ce7fa30b5c0f4697d3813e6cea825d0487`  
		Last Modified: Tue, 04 Jul 2023 15:38:48 GMT  
		Size: 20.9 MB (20872213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d88a941b2ba0fb82a305de45e6388d43fe667b306beaa91ca94a067cb40fd4`  
		Last Modified: Tue, 04 Jul 2023 15:38:57 GMT  
		Size: 191.4 MB (191403784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d551b8b13ca94b247387cfb2cbb37e5a9667e98e83d7912fd82995c5c200dc`  
		Last Modified: Tue, 04 Jul 2023 15:38:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2998f42efdee91326f564135bc45112214b028c1c7abba827d2dcc35dace7113`  
		Last Modified: Wed, 05 Jul 2023 03:16:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38cd1421105c6db47d7d60632b379889b0611971ff25d3653e11ada730a75e7`  
		Last Modified: Wed, 05 Jul 2023 03:21:27 GMT  
		Size: 11.9 MB (11858765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969a0188422fbffcd160b5f11f3c9014277822050b11b738b6796c6551e7dc77`  
		Last Modified: Wed, 05 Jul 2023 03:21:26 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:10c75b4a5a04651f8cb3498b62be92a6ae43683f9960ede91faeef55c5821023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259335615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54296f7dc76d57329ee3ec06b6de14765cce67a782750538b247ed80cbe6e120`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:24 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:25 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:28 GMT
ADD file:0a2372ac4d43f0f4ada2b55dd0a359df73a828a9aa9426bfdd05a02b9c4b2bd9 in / 
# Mon, 05 Jun 2023 17:08:28 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:17:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:17:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:17:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:23:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:23:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 02:23:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:23:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:23:58 GMT
CMD ["jshell"]
# Fri, 16 Jun 2023 07:54:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 16 Jun 2023 07:54:23 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 07:54:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 16 Jun 2023 07:54:35 GMT
WORKDIR /usr/local/tomcat
# Fri, 16 Jun 2023 07:54:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 07:54:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 08:10:27 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 16 Jun 2023 08:10:27 GMT
ENV TOMCAT_MAJOR=8
# Fri, 16 Jun 2023 08:10:28 GMT
ENV TOMCAT_VERSION=8.5.90
# Fri, 16 Jun 2023 08:10:28 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Fri, 16 Jun 2023 08:11:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Fri, 16 Jun 2023 08:11:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 16 Jun 2023 08:11:55 GMT
EXPOSE 8080
# Fri, 16 Jun 2023 08:11:56 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1fbda4a01aa9e184a223c30ab58441354cde30fe3083bc1d8ca9f7823ab4fe68`  
		Last Modified: Fri, 16 Jun 2023 01:24:20 GMT  
		Size: 33.3 MB (33309776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad609b0dd14d25a533bad107d7d80f6a0143d184f80e43339a78811d5d58f6`  
		Last Modified: Fri, 16 Jun 2023 02:29:46 GMT  
		Size: 22.1 MB (22128326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ce741cc8ac3014cd9e49c97fca407822843eea1eb86758faff59dedae1e5ab`  
		Last Modified: Fri, 16 Jun 2023 02:30:05 GMT  
		Size: 192.0 MB (191966187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fe57190c0533e82571289feef9540faa84ed6bc49ac61bdefe97bf38415b96`  
		Last Modified: Fri, 16 Jun 2023 02:29:40 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dfd025af6fb1e907d50e5e95fa1cc1dac4db57387060f8090294801f829387`  
		Last Modified: Fri, 16 Jun 2023 08:28:04 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8997844b4872d370821618372480a56358591bd8d3baf7ebfa2e2525824b2d9`  
		Last Modified: Fri, 16 Jun 2023 08:32:20 GMT  
		Size: 11.9 MB (11930850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb047092076320f9d38c2feb5b1d2314007f9072e0f0943810a161411a9002b`  
		Last Modified: Fri, 16 Jun 2023 08:32:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:b4f6ca86564557f9030e4503d5c056b94c41d3f738c53f6ceaecd5b4cbaed6cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238852251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee4d25937685a2c35e27b14ded16e461180e888ad0d0b47eff7864d6a793bfb`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:58 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:58 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:00 GMT
ADD file:3aeae4efd27981f5d9d2894756f698b4fab4fbc6de4258ebd03baad8bf626d5c in / 
# Mon, 05 Jun 2023 17:08:00 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 18:18:32 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 18:18:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 18:18:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 18:21:06 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 18:21:07 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Fri, 16 Jun 2023 18:21:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 18:21:21 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 18:21:21 GMT
CMD ["jshell"]
# Sat, 17 Jun 2023 10:57:41 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 17 Jun 2023 10:57:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 17 Jun 2023 10:57:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 17 Jun 2023 10:57:42 GMT
WORKDIR /usr/local/tomcat
# Sat, 17 Jun 2023 10:57:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 17 Jun 2023 10:57:42 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 17 Jun 2023 11:01:08 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 17 Jun 2023 11:01:08 GMT
ENV TOMCAT_MAJOR=8
# Sat, 17 Jun 2023 11:01:09 GMT
ENV TOMCAT_VERSION=8.5.90
# Sat, 17 Jun 2023 11:01:09 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Sat, 17 Jun 2023 11:01:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 17 Jun 2023 11:01:34 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 17 Jun 2023 11:01:35 GMT
EXPOSE 8080
# Sat, 17 Jun 2023 11:01:35 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bb7140b141bfafcc2950b11e56e5cb2fe27bf5fd81e61bd4bae6ad3d9b97a085`  
		Last Modified: Fri, 16 Jun 2023 18:23:16 GMT  
		Size: 27.0 MB (27013970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a14b6349235bf7faba275b3805009d19172e7d23b4f8d32be34f0ea9e869d2`  
		Last Modified: Fri, 16 Jun 2023 18:24:20 GMT  
		Size: 19.6 MB (19598167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68642196d6f2d9cde833a2bbe7ff45d306efa1950fcabf9290578035819b23aa`  
		Last Modified: Fri, 16 Jun 2023 18:24:29 GMT  
		Size: 180.4 MB (180363037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628442b5e233a5113b7ddec1cdcdfe873713309b7b61a81dd41bec36ed5fb38a`  
		Last Modified: Fri, 16 Jun 2023 18:24:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a7d17fc2664efe43ee54b3f52851c3356bd8e9fc38c17dba8c4671e2c3d62`  
		Last Modified: Sat, 17 Jun 2023 11:06:53 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1355f350bf8ac128b3fdf0c17049d969ea75bd94801735baba579dd840ccff`  
		Last Modified: Sat, 17 Jun 2023 11:08:17 GMT  
		Size: 11.9 MB (11876602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a94e2acdaefb935c255f96c7616233878b21bbf84072fa5b22f310add5fc17f`  
		Last Modified: Sat, 17 Jun 2023 11:08:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
