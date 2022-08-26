## `tomcat:8-jre11-temurin-jammy`

```console
$ docker pull tomcat@sha256:6dd343fcf55eb2e15ad2df3a5f8ff0c2c6c06fa57afc18cf8784112fa27174c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre11-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:5c613666039dd3e7dd8ab246102c09ec418dbeb6b6b219daa561fbc335ae6a04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101035659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a7056025c0f37fea10363de8acc08e00471429f0809792cf861aa7426dd502`
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
# Wed, 24 Aug 2022 19:20:36 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:21:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:21:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 22:06:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 22:06:28 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 22:06:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 22:06:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 22:06:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 22:06:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 22:15:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 24 Aug 2022 22:15:55 GMT
ENV TOMCAT_MAJOR=8
# Wed, 24 Aug 2022 22:15:55 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 24 Aug 2022 22:15:55 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 24 Aug 2022 22:15:55 GMT
COPY dir:5c7e7d927f837ebaa7da0f9d9bf30c3ed31b1539cc495b02394aacc8492b1b3b in /usr/local/tomcat 
# Wed, 24 Aug 2022 22:15:59 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 22:16:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 22:16:00 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 22:16:01 GMT
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
	-	`sha256:038f6850cd14793dfe8f7ad5b44ffe6450a213068e067d07d0cf596142a6e79b`  
		Last Modified: Wed, 24 Aug 2022 19:28:04 GMT  
		Size: 46.5 MB (46498569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904c98e207563182da3e2d2dc0807b12c9456b51c902b8a29e3e59acc925e909`  
		Last Modified: Wed, 24 Aug 2022 19:27:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd424e54764dba0923d1efd0cd69b9e3cbcc8aed682152775e2ecb8bc0958a9`  
		Last Modified: Wed, 24 Aug 2022 22:23:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01972b4acbf5fa2bbd79019457a2916580f63686187c344dbd37118781fbb8c5`  
		Last Modified: Wed, 24 Aug 2022 22:33:23 GMT  
		Size: 11.2 MB (11202348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b95fc733619f00d30f6b7a4de77b494ff5c7c4a3056e2b828eeeb06f00cfc7`  
		Last Modified: Wed, 24 Aug 2022 22:33:22 GMT  
		Size: 452.1 KB (452140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81a68743f4e6e7442a4e304bc5ce8b21705f158c1fb6b15e49e836544189fc7`  
		Last Modified: Wed, 24 Aug 2022 22:33:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:729e67948a3b3e3cb7c51e59d7e782412a3ed959dd663556f8a3552395d1a1d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95288267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc5031a5062641d70e9b1d0cfa76b4ee9f827e3add78ac4c2e76e1f76043b82`
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
# Thu, 25 Aug 2022 13:23:14 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Thu, 25 Aug 2022 13:24:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 25 Aug 2022 13:24:02 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 26 Aug 2022 03:26:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 26 Aug 2022 03:26:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Aug 2022 03:26:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 26 Aug 2022 03:26:01 GMT
WORKDIR /usr/local/tomcat
# Fri, 26 Aug 2022 03:26:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 26 Aug 2022 03:26:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 26 Aug 2022 03:42:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 26 Aug 2022 03:42:55 GMT
ENV TOMCAT_MAJOR=8
# Fri, 26 Aug 2022 03:42:55 GMT
ENV TOMCAT_VERSION=8.5.82
# Fri, 26 Aug 2022 03:42:55 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Fri, 26 Aug 2022 03:42:57 GMT
COPY dir:89ac32261d422188e99b69650e90120a756460d3ea9df4ef2f3ef50a9edc362d in /usr/local/tomcat 
# Fri, 26 Aug 2022 03:43:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Aug 2022 03:43:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 26 Aug 2022 03:43:08 GMT
EXPOSE 8080
# Fri, 26 Aug 2022 03:43:08 GMT
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
	-	`sha256:647f7495fc30f7f2da04f2a54638800f67874cfb6b6aab4150d622c18894632b`  
		Last Modified: Thu, 25 Aug 2022 13:30:28 GMT  
		Size: 44.7 MB (44674954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4934e04998b49310d6c38ebaf325b8cb3868c62b859752bf10a38921d2a42d2`  
		Last Modified: Thu, 25 Aug 2022 13:30:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d50451f20d2723e8a8ae7cda064523db6b63afc1974fcc57af4e3c0d393e871`  
		Last Modified: Fri, 26 Aug 2022 03:59:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d95137f69676dfa240d4a590bff494fe37581fcf49f9584ddd1c69b89b7a4be`  
		Last Modified: Fri, 26 Aug 2022 04:13:21 GMT  
		Size: 11.1 MB (11135330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baed4947b3e2af1896898c64cb027d9b711d179d45c54b82791c9d2edbd41ded`  
		Last Modified: Fri, 26 Aug 2022 04:13:20 GMT  
		Size: 426.6 KB (426560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e77591f91cd55f61ac4f2985e6b665546a320297aa6dfb58edfcf4f93cfbd66`  
		Last Modified: Fri, 26 Aug 2022 04:13:19 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:0c2f8d557a98802a7ca321e56cf09a81af86670ec049773e0953b6ebdf328abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97044119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2383f8ab0e8c75634397f2d2d48b1f9b2a6c0e5552bc2bbe1081b96b33c5de8c`
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
# Wed, 24 Aug 2022 19:41:05 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:41:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:41:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 21:20:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 21:20:21 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 21:20:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 21:20:23 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 21:20:24 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 21:20:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 21:36:06 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 24 Aug 2022 21:36:06 GMT
ENV TOMCAT_MAJOR=8
# Wed, 24 Aug 2022 21:36:07 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 24 Aug 2022 21:36:08 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 24 Aug 2022 21:36:10 GMT
COPY dir:bba3082b786e828cbcad6101489d8d52f7422f08093a0adf78bd0264b0c058e6 in /usr/local/tomcat 
# Wed, 24 Aug 2022 21:36:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 21:36:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 21:36:19 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 21:36:20 GMT
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
	-	`sha256:042d81bb6b9272594d41df4317c8cf379d5be12ec7996d43c3ff4895df8f7481`  
		Last Modified: Wed, 24 Aug 2022 19:48:46 GMT  
		Size: 44.8 MB (44826689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43604d6aa5b7375e91eff36fad8ec1318a6778b92030981be3df7a05dd83427`  
		Last Modified: Wed, 24 Aug 2022 19:48:39 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f4ffb2ea5560a3bd73f2a4330ac7bb7ac6fa090a621775164836bad8d7b6b7`  
		Last Modified: Wed, 24 Aug 2022 21:49:52 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b71b9a73def6eaee52391b5099ee99d7fdd8e6568fc2ae1d1496001dc0ba80`  
		Last Modified: Wed, 24 Aug 2022 22:02:17 GMT  
		Size: 11.2 MB (11207227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907ed77db91b8a9161874f4878ea33e6c19b6a80f868532e9623398e668331d`  
		Last Modified: Wed, 24 Aug 2022 22:02:16 GMT  
		Size: 214.4 KB (214399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:ec8692491169d8ccb9536e9cea2daa54530d5394f2d1f518e56814f9982a70d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102600013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:caecbd1225f7ac180790c28fb2f28dd7f64008f99e5283b1a16c47a4fb148ab7`
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
# Wed, 24 Aug 2022 19:17:57 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:19:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:19:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 20:16:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 20:16:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 20:16:36 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 20:16:36 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 20:16:37 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 20:16:37 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 20:35:09 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 24 Aug 2022 20:35:09 GMT
ENV TOMCAT_MAJOR=8
# Wed, 24 Aug 2022 20:35:10 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 24 Aug 2022 20:35:10 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 24 Aug 2022 20:35:11 GMT
COPY dir:9c43a8e05655341c8a3b9d4837ae0d08b44fd3462fe3def824e0b3c017fc4908 in /usr/local/tomcat 
# Wed, 24 Aug 2022 20:35:19 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 20:35:21 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 20:35:21 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 20:35:22 GMT
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
	-	`sha256:11dde1754fff5ab26a7a3c2d0c69cc3d4f446be3005c4f3241efc7299d7a4fd5`  
		Last Modified: Wed, 24 Aug 2022 19:27:56 GMT  
		Size: 41.9 MB (41884755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7c108ed376a4e523fb24aef9662f54fffa0bdf15b312c8db1b279cf50c39a6`  
		Last Modified: Wed, 24 Aug 2022 19:27:46 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071b8ff5d7f3c09346feec6a0e6077b4d8ee646dc1a545d7607e7bec650cddd`  
		Last Modified: Wed, 24 Aug 2022 20:48:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32557facf1e13c1cdb81c022aff23c9fce1be8f9ee248f4cef23676b3c0c51f`  
		Last Modified: Wed, 24 Aug 2022 21:02:11 GMT  
		Size: 11.2 MB (11229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c18445990bd5b4282474f0e839aa5b5b823164945ef0ded71f949beeeec308e`  
		Last Modified: Wed, 24 Aug 2022 21:02:09 GMT  
		Size: 483.5 KB (483453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b501139bcfd4045b03add77ae6b21834321a3a97eaf5a9ff0e0919172aeea2a`  
		Last Modified: Wed, 24 Aug 2022 21:02:09 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:11edd24353591118bdbc171ee53eb4cd2b71ae078305bd9ec4d9c8b60810d572
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93292224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5484c7d70e57eb9fff16399f74eb153ad16918c6aa598991e3c788c9b16bcf`
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
# Wed, 24 Aug 2022 19:42:16 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:43:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:43:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 20:54:35 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 20:54:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 20:54:35 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 20:54:36 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 20:54:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 20:54:36 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 21:05:36 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 24 Aug 2022 21:05:36 GMT
ENV TOMCAT_MAJOR=8
# Wed, 24 Aug 2022 21:05:37 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 24 Aug 2022 21:05:37 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 24 Aug 2022 21:05:37 GMT
COPY dir:996bee6d4a0fcdbfcd17684627e3eb3fcefb169f2fcbbe65a6245c863016eaab in /usr/local/tomcat 
# Wed, 24 Aug 2022 21:05:40 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 21:05:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 21:05:42 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 21:05:42 GMT
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
	-	`sha256:89ff9ae8e8e505b4ed92732195fec6bcfdc0d387cb9f0301bfa916cef314274a`  
		Last Modified: Wed, 24 Aug 2022 19:52:56 GMT  
		Size: 40.5 MB (40479764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33a185909339114744e2fdb5f5ad23d800fc7d6c2c6190c053c0c40475d7289`  
		Last Modified: Wed, 24 Aug 2022 19:52:47 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1312b5c7728ea33a92826e0d015061c8fb7a62c7b07f3557153da0593139027b`  
		Last Modified: Wed, 24 Aug 2022 21:27:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a736756d83fec71c1e3ab11520eb50af8bc2af7a932ebce19373e0df41e80`  
		Last Modified: Wed, 24 Aug 2022 21:33:53 GMT  
		Size: 11.2 MB (11196608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652263f425a4a5ef796c30b2baf0c9eadcf874ba64f3a728c2b4e31181a941c5`  
		Last Modified: Wed, 24 Aug 2022 21:33:53 GMT  
		Size: 453.7 KB (453689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb6fb6646dec9976fbe83e01fa786232f619b18655079ed0c957105548bf59`  
		Last Modified: Wed, 24 Aug 2022 21:33:53 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
