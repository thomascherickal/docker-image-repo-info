## `tomcat:8-jdk11-temurin-jammy`

```console
$ docker pull tomcat@sha256:08fd0a286212d0c6095f58d66f8dd65f558c4db9a6e3d9fdda28cd3d52fc2dbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jdk11-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:03c6519baa604417fd4dd7f01a29b5791710a61f9866d46ed024ade203b3c3f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252678741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76f7db3f29ff179f047c98793eaa86359a2ebd5a80b3119cd6288867a902ded`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:20:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:20:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:20:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Aug 2022 17:22:09 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Fri, 12 Aug 2022 17:22:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bb345cabf3e305ff3ce390918d5f69e5cfbced3d9844e0b0531c2690f9ed06ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='2b0b390ba17963d70883506a72b58d315cab7a24b418fdab5351728f328f398e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='40dea12da26443ad731f9348187b65451711659337e83b6409a2bcf0f057cd2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f7975c9670a6697d0afedd3ebebe545f04bdec9aa7efbe9136f1c5182eca62e1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f79506f80c796d8e6a382f00bd8c528a330c5e29581aaf5cb61e1831742d166f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 12 Aug 2022 17:22:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 12 Aug 2022 17:22:20 GMT
CMD ["jshell"]
# Fri, 12 Aug 2022 20:14:25 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 20:14:25 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 20:14:26 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 20:14:26 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 20:14:26 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 20:14:26 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 20:27:37 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 20:27:37 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:28:07 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:28:08 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:28:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 17 Aug 2022 21:28:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:28:43 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:28:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65811de5a1ce73e051835187b84371fd526024c2be009224c3a1f5adaa87c90`  
		Last Modified: Fri, 12 Aug 2022 17:28:31 GMT  
		Size: 12.5 MB (12456003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075d0c0e8bbb371e8dd0998a6df9602147fa94aaa29ea0c24a7e6579b879dd2b`  
		Last Modified: Fri, 12 Aug 2022 17:30:38 GMT  
		Size: 198.1 MB (198127118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8180b0c10f0e630efdfd7f7c94abba72a9cd8bf274c38592a8f60ff13285ac2`  
		Last Modified: Fri, 12 Aug 2022 17:30:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8833dbc8a999b9cf129944d8f924b4e0000f1efe561d71194cebee5e03c566`  
		Last Modified: Fri, 12 Aug 2022 20:40:19 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdd00be9997919dd9a14385521028f773fe471a52d6da9f459cda1761bcd0d5`  
		Last Modified: Wed, 17 Aug 2022 21:51:52 GMT  
		Size: 11.7 MB (11669009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2cbfeff2fb6dbccb057816c0da5b06f39f59dcf9b119eb548923949934969`  
		Last Modified: Wed, 17 Aug 2022 21:51:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk11-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:4f397ea74d23a7dd133a2fdc40e6172547fcd7c114e7ffff242eeef45b82e550
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.2 MB (236171166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa62d31de3dc7c6a372d9a6610efce5f3d5472eb64059f1e5f18e46eb3e7a14`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:56 GMT
ADD file:1bec4ea562c9a42add30f5e3626edc93bdfc0271cbd208a4447842fa31b5c114 in / 
# Tue, 02 Aug 2022 01:40:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:58:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:58:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:58:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 16:58:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Aug 2022 16:59:50 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Fri, 12 Aug 2022 16:59:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bb345cabf3e305ff3ce390918d5f69e5cfbced3d9844e0b0531c2690f9ed06ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='2b0b390ba17963d70883506a72b58d315cab7a24b418fdab5351728f328f398e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='40dea12da26443ad731f9348187b65451711659337e83b6409a2bcf0f057cd2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f7975c9670a6697d0afedd3ebebe545f04bdec9aa7efbe9136f1c5182eca62e1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f79506f80c796d8e6a382f00bd8c528a330c5e29581aaf5cb61e1831742d166f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 12 Aug 2022 17:00:02 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 12 Aug 2022 17:00:02 GMT
CMD ["jshell"]
# Fri, 12 Aug 2022 18:16:12 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 18:16:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 18:16:12 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 18:16:12 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 18:16:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:16:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:32:46 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 18:32:47 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:05:40 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:05:40 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:06:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 17 Aug 2022 21:06:25 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:06:25 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:06:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1a5cf9a21e485b0a676c22ced0e80a140055b3ef0d7573caf5be408a10ddb04`  
		Last Modified: Tue, 02 Aug 2022 01:43:32 GMT  
		Size: 27.0 MB (27017015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f750e2d5f8b88349d4851becd87f9216149478e46f3c5da8cf34b92d6cf5975d`  
		Last Modified: Fri, 12 Aug 2022 17:06:31 GMT  
		Size: 12.0 MB (12033944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab82de343dcefdbbe437658b67e3e7a95f0b730380449985e75a62ea6d37276`  
		Last Modified: Fri, 12 Aug 2022 17:08:14 GMT  
		Size: 185.5 MB (185543377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e87c3986899c0841d1a633a7ff9eb5e8fc310e55c5d146ff300b6d321a0f6da`  
		Last Modified: Fri, 12 Aug 2022 17:07:58 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0ff032ca7605f0c261ba646fb99b2a579bce32a02c8618ae9018e6adbad2b`  
		Last Modified: Fri, 12 Aug 2022 18:49:04 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8973c04c3b56cc5146b94c3bcc2227e23101605fefc209de0eb3dd3bf1384`  
		Last Modified: Wed, 17 Aug 2022 21:25:38 GMT  
		Size: 11.6 MB (11576350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2475c8ccfe19b4cb08117fab255c4d4b05c572087a63670b163bce89e48c762`  
		Last Modified: Wed, 17 Aug 2022 21:25:37 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk11-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:2048e0fb5759fe206a91430d7d33366c1fcefeaea09d2c3d32e78a3ce96d977a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.1 MB (247106251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9feca0c1a23218f06ea08857169078d2b692b57c6c20cd396cef9dc7810083e8`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:40:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:40:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:40:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:40:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Aug 2022 17:42:38 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Fri, 12 Aug 2022 17:42:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bb345cabf3e305ff3ce390918d5f69e5cfbced3d9844e0b0531c2690f9ed06ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='2b0b390ba17963d70883506a72b58d315cab7a24b418fdab5351728f328f398e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='40dea12da26443ad731f9348187b65451711659337e83b6409a2bcf0f057cd2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f7975c9670a6697d0afedd3ebebe545f04bdec9aa7efbe9136f1c5182eca62e1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f79506f80c796d8e6a382f00bd8c528a330c5e29581aaf5cb61e1831742d166f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 12 Aug 2022 17:42:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 12 Aug 2022 17:42:50 GMT
CMD ["jshell"]
# Fri, 12 Aug 2022 21:16:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 21:16:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 21:16:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 21:16:52 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 21:16:53 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 21:16:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 21:39:53 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 21:39:54 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 22:00:25 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 22:00:25 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 22:01:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 17 Aug 2022 22:01:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 22:01:11 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 22:01:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a729bc90f861d8ccd964a45b6f12093afcb2172c43390409a73e938d36aa1a`  
		Last Modified: Fri, 12 Aug 2022 17:51:29 GMT  
		Size: 12.4 MB (12414351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec2b62bb819ab1ee20c914d19a6e9b382fc7c9012ee1ab76044ba9dc310aeaa`  
		Last Modified: Fri, 12 Aug 2022 17:53:51 GMT  
		Size: 194.9 MB (194871695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0066ef97851172ac99d0a121842b1aabc767a28004d2d77a2aae6c80c4cf0771`  
		Last Modified: Fri, 12 Aug 2022 17:53:34 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6492a0fb716513380547132f3701a3ca6c24caa29f1b98c20052d6f93e6450`  
		Last Modified: Fri, 12 Aug 2022 22:04:15 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc67f417465f3e66dc4f7669711dc6fdb919efec99552397dce3c1e930e7149`  
		Last Modified: Wed, 17 Aug 2022 22:40:13 GMT  
		Size: 11.4 MB (11438754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk11-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:f9f0f03c7434744f07870607a082e692b75123dd4982c7c8f210bc79c36e406a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.8 MB (240762412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c901679bd7b663ee65f6a72661d107f46bb7bba548e39fe296eff8b1644a191a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:17:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:18:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:18:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:18:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Aug 2022 17:21:19 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Fri, 12 Aug 2022 17:21:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bb345cabf3e305ff3ce390918d5f69e5cfbced3d9844e0b0531c2690f9ed06ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='2b0b390ba17963d70883506a72b58d315cab7a24b418fdab5351728f328f398e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='40dea12da26443ad731f9348187b65451711659337e83b6409a2bcf0f057cd2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f7975c9670a6697d0afedd3ebebe545f04bdec9aa7efbe9136f1c5182eca62e1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f79506f80c796d8e6a382f00bd8c528a330c5e29581aaf5cb61e1831742d166f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 12 Aug 2022 17:21:42 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 12 Aug 2022 17:21:43 GMT
CMD ["jshell"]
# Fri, 12 Aug 2022 18:30:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 18:30:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 18:30:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 18:30:58 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 18:30:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:30:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:54:24 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 18:54:24 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:26:48 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:26:48 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:27:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 17 Aug 2022 21:27:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:27:57 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:27:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fcd220292d9dad8eb173395ef5248eff48a8e454b824073126548d8a30db0a`  
		Last Modified: Fri, 12 Aug 2022 17:33:11 GMT  
		Size: 13.3 MB (13283444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faad34bbfa68e92239797c94b9e8ce6c0b9551cc121afe711cd62d9cfdb9a2b`  
		Last Modified: Fri, 12 Aug 2022 17:36:10 GMT  
		Size: 180.0 MB (180033680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c9a9c84c6b16032e56592922ba9200a981e954c0797d9625d491dd528fcc4b`  
		Last Modified: Fri, 12 Aug 2022 17:35:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5b0838914dd240ba075ad5d7ed3e0bd4dc74287860d82c1939b06af0ca086c`  
		Last Modified: Fri, 12 Aug 2022 19:11:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bf28ed02702ac704b4b1170e975c660665570d27ac9f162aae34e493e2e7ae`  
		Last Modified: Wed, 17 Aug 2022 21:47:08 GMT  
		Size: 11.7 MB (11726808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014972326c586dc2ad5393806683eb61db4d078a08ad94128a71b00780474b2a`  
		Last Modified: Wed, 17 Aug 2022 21:47:07 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk11-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:087b5bc39d8cd4bbd7e42af8cc5962824332786159f11f6c5c73f941b4cfe88f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.1 MB (225088640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb16dd219bc630da65471d91e45f899e9a099fba1abff2a7d1fe0d3a663e0e34`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:42:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:42:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:42:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 12 Aug 2022 17:42:41 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Fri, 12 Aug 2022 17:42:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bb345cabf3e305ff3ce390918d5f69e5cfbced3d9844e0b0531c2690f9ed06ef';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='2b0b390ba17963d70883506a72b58d315cab7a24b418fdab5351728f328f398e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='40dea12da26443ad731f9348187b65451711659337e83b6409a2bcf0f057cd2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f7975c9670a6697d0afedd3ebebe545f04bdec9aa7efbe9136f1c5182eca62e1';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f79506f80c796d8e6a382f00bd8c528a330c5e29581aaf5cb61e1831742d166f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 12 Aug 2022 17:42:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 12 Aug 2022 17:42:58 GMT
CMD ["jshell"]
# Fri, 12 Aug 2022 18:39:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 18:39:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 18:39:53 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 18:39:54 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 18:39:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:39:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:50:50 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 18:50:50 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:49:01 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:49:02 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:49:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 17 Aug 2022 21:49:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:49:58 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:49:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b487214c25e1024a8781e65f9a2199413fa526aee2b0ad57feec90899ac822c`  
		Last Modified: Fri, 12 Aug 2022 17:48:54 GMT  
		Size: 12.5 MB (12518919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9191eacd184c568648eb52e629571311406cf85ee25a7ba1c5a5678952d7296`  
		Last Modified: Fri, 12 Aug 2022 17:49:04 GMT  
		Size: 172.3 MB (172259778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc2ec8d8682931227df807dd763ac182ef32a6903a08a1336d1fb62e34e75b6`  
		Last Modified: Fri, 12 Aug 2022 17:48:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94ea1111b5d8ddec6d1381c30c0d4e015cc581280a5a5a4d011d4d8241848df`  
		Last Modified: Fri, 12 Aug 2022 19:00:36 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f177d4dfa614ab9b9b2c12762d6a0a8ef74003fb8e4575b02e08669c27fcd0da`  
		Last Modified: Wed, 17 Aug 2022 22:01:59 GMT  
		Size: 11.7 MB (11666681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3f5cf88a217739dce3438df2cabdf61604ec4370f24a5d71faf1bc91727664`  
		Last Modified: Wed, 17 Aug 2022 22:01:58 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
