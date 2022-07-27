## `tomcat:8-jre11-temurin-focal`

```console
$ docker pull tomcat@sha256:585348c67d27a7fccf156d6e89002d64860562b4fb7d6963d38dff9e68c7c13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre11-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:ea09b248abc15bd0acfcc9ae2ac74b34cd3f7a7e289b3e67b22a5957f4591faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101482617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ec8c6c9cb7b314df59d1d0efc3e5bbbd1e28a1fbbf30a26f3e108a6088998d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:12:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:14:23 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 07 Jun 2022 00:14:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a9e1b9fcef7c2fa9911bd9f2bf51591102ee0367a667e154cf15f20d0c6faa6a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.15_10.tar.gz';          ;;        armhf|arm)          ESUM='12489d268a6758dc72c073b11a25eb494804649f4760db05b2ef9ddb71aab73e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.15_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd0fad840c3aa118c0ab4cf4070cb9ad25c0ccab456aa22f9b5fc02f4230b26a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.15_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d371ecceccf1d807ca9f0721dba805c65dddc9c5e59c5faaabad37f191970745';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.15_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='22831fd097dfb39e844cb34f42064ff26a0ada9cd13621d7b8bca8e9b9d3a5ee';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:14:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:14:59 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 06:30:41 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 06:30:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:30:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 06:30:41 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 06:30:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 06:30:42 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 06:39:10 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 07 Jun 2022 06:39:10 GMT
ENV TOMCAT_MAJOR=8
# Mon, 13 Jun 2022 20:31:09 GMT
ENV TOMCAT_VERSION=8.5.81
# Mon, 13 Jun 2022 20:31:09 GMT
ENV TOMCAT_SHA512=729387275cce4a0900289722f6c70ebcf7aee924af671b110b8ea8577fd6d045d47f17d526c8db5fd41c8590102e7f5100e95e89f7fd511b941565812ecbed35
# Fri, 22 Jul 2022 03:14:07 GMT
COPY dir:830f44c670af2b9dc350c6b97d62401d3f807aedc80be686326c452fb8fd55b2 in /usr/local/tomcat 
# Fri, 22 Jul 2022 03:14:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Jul 2022 03:14:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 Jul 2022 03:14:13 GMT
EXPOSE 8080
# Fri, 22 Jul 2022 03:14:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caca7a4a00fe7d5efa72ecdbb346c7a4ee0e8e43c3a263d2bb79893d52bd4678`  
		Last Modified: Tue, 07 Jun 2022 00:19:21 GMT  
		Size: 16.0 MB (16029798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b669251e19038a24bd6cab0baab92077f23163880fac4701fb3efa564350732b`  
		Last Modified: Tue, 07 Jun 2022 00:21:34 GMT  
		Size: 43.3 MB (43267270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf45eff8a02bcdf7a96904e0dc534c78c89a5c860e224fa57780ef2fc2eab99e`  
		Last Modified: Tue, 07 Jun 2022 00:21:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246089a07769500a0adb027d1dc0efbb1254ee07d75dcdc6f8a3ceb8bae3e95f`  
		Last Modified: Tue, 07 Jun 2022 06:48:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd6ada0285876e56496c1555ead5b30db5b5e107b145ee82fc892255819b186`  
		Last Modified: Fri, 22 Jul 2022 03:59:06 GMT  
		Size: 11.3 MB (11260380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a236c8af0b63064de1aa1ad830a71d5ac82b2e134df11bb72cc45bb5d32a2cc1`  
		Last Modified: Fri, 22 Jul 2022 03:59:06 GMT  
		Size: 2.4 MB (2352074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181ea11cdb8edf6e0603cf1c6605d56a3c596e97c4c69c7c8dbd411ce92b0c12`  
		Last Modified: Fri, 22 Jul 2022 03:59:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:f9aaa5c3cfc4f2a4ce010aa1a8ff41654573e502a00893ee0ed3cb81b72939db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94563617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f488be68abaae3e2c31cf58d82ea4f520e3328f216083a99d9e9252d66446dbd`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:33:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 09:34:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:38:26 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 07 Jun 2022 09:40:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a9e1b9fcef7c2fa9911bd9f2bf51591102ee0367a667e154cf15f20d0c6faa6a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.15_10.tar.gz';          ;;        armhf|arm)          ESUM='12489d268a6758dc72c073b11a25eb494804649f4760db05b2ef9ddb71aab73e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.15_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd0fad840c3aa118c0ab4cf4070cb9ad25c0ccab456aa22f9b5fc02f4230b26a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.15_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d371ecceccf1d807ca9f0721dba805c65dddc9c5e59c5faaabad37f191970745';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.15_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='22831fd097dfb39e844cb34f42064ff26a0ada9cd13621d7b8bca8e9b9d3a5ee';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:40:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:40:12 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 27 Jul 2022 11:12:25 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 27 Jul 2022 11:12:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 11:12:26 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 27 Jul 2022 11:12:26 GMT
WORKDIR /usr/local/tomcat
# Wed, 27 Jul 2022 11:12:26 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 11:12:26 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 11:29:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 27 Jul 2022 11:29:21 GMT
ENV TOMCAT_MAJOR=8
# Wed, 27 Jul 2022 11:29:21 GMT
ENV TOMCAT_VERSION=8.5.81
# Wed, 27 Jul 2022 11:29:21 GMT
ENV TOMCAT_SHA512=729387275cce4a0900289722f6c70ebcf7aee924af671b110b8ea8577fd6d045d47f17d526c8db5fd41c8590102e7f5100e95e89f7fd511b941565812ecbed35
# Wed, 27 Jul 2022 11:29:22 GMT
COPY dir:839bb6049071abba731d66f54481855c61f05840a7a0c3705ab1a1684702623e in /usr/local/tomcat 
# Wed, 27 Jul 2022 11:29:30 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 11:29:32 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 11:29:32 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 11:29:32 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ae1d24c2862f98f09de4a24a053161044e470b33c4e92d9f9807726bf4d12d`  
		Last Modified: Tue, 07 Jun 2022 09:51:03 GMT  
		Size: 14.9 MB (14902076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc3ad5b6919924f1b64370d624d55a826023a17770911288544d2b1ea240fcb`  
		Last Modified: Tue, 07 Jun 2022 09:57:10 GMT  
		Size: 41.9 MB (41886172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e62ed4eea1903635cf0cbb09d90add4fc57f390f08a42d42b281d6bc655e8c8`  
		Last Modified: Tue, 07 Jun 2022 09:56:44 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb3c7f1a6ead0de02942a9b71ae8067a5a103ac12afa0aefc36eb674845a59`  
		Last Modified: Wed, 27 Jul 2022 11:49:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2d95e676d348e6af7e46770a03557ebadcd8df411e89542a065a1a29ceffb2`  
		Last Modified: Wed, 27 Jul 2022 12:01:04 GMT  
		Size: 11.2 MB (11213608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e7c1507bae642a8470ce4509d4b3876f63a6ac3c1954a3046d3c7e23ddb6c9`  
		Last Modified: Wed, 27 Jul 2022 12:01:03 GMT  
		Size: 2.0 MB (1968659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea473eaccb293b5c2fcc3c2e3c993574894b5058cf76faac7973a4c67b3cca`  
		Last Modified: Wed, 27 Jul 2022 12:01:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:c0937ddf79a4ff4cc0303a8ab632769472ae721c7ff6bae0effa462ea8cc6406
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.2 MB (98193279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faea00fa06c9011408ba4f971beb8127bf6124db4abd09586a61ab465c152b2d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:59:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 05:00:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:35:32 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 07 Jun 2022 06:36:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a9e1b9fcef7c2fa9911bd9f2bf51591102ee0367a667e154cf15f20d0c6faa6a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.15_10.tar.gz';          ;;        armhf|arm)          ESUM='12489d268a6758dc72c073b11a25eb494804649f4760db05b2ef9ddb71aab73e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.15_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd0fad840c3aa118c0ab4cf4070cb9ad25c0ccab456aa22f9b5fc02f4230b26a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.15_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d371ecceccf1d807ca9f0721dba805c65dddc9c5e59c5faaabad37f191970745';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.15_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='22831fd097dfb39e844cb34f42064ff26a0ada9cd13621d7b8bca8e9b9d3a5ee';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:36:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:36:20 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 10:50:03 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 10:50:03 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 10:50:04 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 10:50:05 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 10:50:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:50:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 11:04:44 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 07 Jun 2022 11:04:44 GMT
ENV TOMCAT_MAJOR=8
# Mon, 13 Jun 2022 21:21:56 GMT
ENV TOMCAT_VERSION=8.5.81
# Mon, 13 Jun 2022 21:21:57 GMT
ENV TOMCAT_SHA512=729387275cce4a0900289722f6c70ebcf7aee924af671b110b8ea8577fd6d045d47f17d526c8db5fd41c8590102e7f5100e95e89f7fd511b941565812ecbed35
# Fri, 22 Jul 2022 04:23:09 GMT
COPY dir:f01f7179453aad967a908c4f7991a9c4f86a6fbcb12c0069ea2c1559e031c464 in /usr/local/tomcat 
# Fri, 22 Jul 2022 04:23:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Jul 2022 04:23:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 Jul 2022 04:23:19 GMT
EXPOSE 8080
# Fri, 22 Jul 2022 04:23:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15da1b4c110f7cc460fbf968fb55b77c541f0e3ab87b92d5e6a822cc2c593e1`  
		Last Modified: Tue, 07 Jun 2022 05:10:23 GMT  
		Size: 15.9 MB (15898299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8e9d6a15d13e6f2d5d43f40b76051350cb7090cfcae5300dc1647e3196577a`  
		Last Modified: Tue, 07 Jun 2022 06:44:15 GMT  
		Size: 41.6 MB (41608356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51219ca7d003431d2f9c6ddda7db0a1902cf2b7e4e879625811b086f268b39c`  
		Last Modified: Tue, 07 Jun 2022 06:44:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aa4900f44b9e3e20168d54fda3a0b78e62d572de1796db20345b70b1d8b3ca`  
		Last Modified: Tue, 07 Jun 2022 11:23:12 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b707d47072a95bf69535d82762c9eb8a98a9a3264263e1d5b76847e53c342c`  
		Last Modified: Fri, 22 Jul 2022 05:24:33 GMT  
		Size: 11.3 MB (11279360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e064cc36351c0020aff1dec0b4adc4df7d83f1215ae784af5a64e8e5146ca0b`  
		Last Modified: Fri, 22 Jul 2022 05:24:32 GMT  
		Size: 2.2 MB (2215788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:b296397c9894f8306c635c2a31936aade344984645b1986d3509a44bafb1bf07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (103024472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527d28cffc7ad64f081f5c0a024e3c370730b05ee1d949e310159f4ed3aa3e55`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:18:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 07:20:45 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 07 Jun 2022 07:22:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a9e1b9fcef7c2fa9911bd9f2bf51591102ee0367a667e154cf15f20d0c6faa6a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.15_10.tar.gz';          ;;        armhf|arm)          ESUM='12489d268a6758dc72c073b11a25eb494804649f4760db05b2ef9ddb71aab73e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.15_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd0fad840c3aa118c0ab4cf4070cb9ad25c0ccab456aa22f9b5fc02f4230b26a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.15_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d371ecceccf1d807ca9f0721dba805c65dddc9c5e59c5faaabad37f191970745';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.15_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='22831fd097dfb39e844cb34f42064ff26a0ada9cd13621d7b8bca8e9b9d3a5ee';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 07:22:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 07:22:29 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 10 Jun 2022 02:41:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 10 Jun 2022 02:42:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jun 2022 02:42:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 10 Jun 2022 02:42:14 GMT
WORKDIR /usr/local/tomcat
# Fri, 10 Jun 2022 02:42:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 10 Jun 2022 02:42:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 10 Jun 2022 03:23:19 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 10 Jun 2022 03:23:27 GMT
ENV TOMCAT_MAJOR=8
# Mon, 13 Jun 2022 22:35:27 GMT
ENV TOMCAT_VERSION=8.5.81
# Mon, 13 Jun 2022 22:35:31 GMT
ENV TOMCAT_SHA512=729387275cce4a0900289722f6c70ebcf7aee924af671b110b8ea8577fd6d045d47f17d526c8db5fd41c8590102e7f5100e95e89f7fd511b941565812ecbed35
# Fri, 22 Jul 2022 06:01:34 GMT
COPY dir:4cf8978697f57b4af6d2f5b445bea1c6b907b256f0a48997458e42b4dcb140d9 in /usr/local/tomcat 
# Fri, 22 Jul 2022 06:02:06 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Jul 2022 06:02:21 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 Jul 2022 06:02:27 GMT
EXPOSE 8080
# Fri, 22 Jul 2022 06:02:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6c621e52fdf1e59e073b1c51c52e2e5a829be92510ef56949c609a03af2492`  
		Last Modified: Tue, 07 Jun 2022 07:30:19 GMT  
		Size: 17.2 MB (17203633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f2b429630df08a83b6aa0750904f47e0c7b5e10beddf858b181db00d37ad41`  
		Last Modified: Tue, 07 Jun 2022 07:31:44 GMT  
		Size: 38.7 MB (38675851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f71d75d88433a018b8733bd57c5f281705c82399d226521b2c2f08a5ece440`  
		Last Modified: Tue, 07 Jun 2022 07:31:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f245fbaf648c1b68b997ac04a279a87e0555b2abd3d6fc79e8d5f30476c11f6`  
		Last Modified: Fri, 10 Jun 2022 03:37:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ce3eb13fb98f36507c04fd8182692ae14be3e5fa956b0acf54fbe7529f3698`  
		Last Modified: Fri, 22 Jul 2022 06:16:02 GMT  
		Size: 11.3 MB (11302421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ff9d5f8a20b4f7919529a685bb6783b21239bd5d2e88187bf57633c1ed76cc`  
		Last Modified: Fri, 22 Jul 2022 06:16:01 GMT  
		Size: 2.5 MB (2547758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d585eaf21d2cbdf456915ae471b3a0d027f86ed82801bbe3d4e4131308ebe941`  
		Last Modified: Fri, 22 Jul 2022 06:16:00 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre11-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:59d0ac904a09b3877307a661ee2d5765bca9bd880bd772b5cd5fc13f1ff4fdf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93477237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da891bb25529551e6716342a0fac196ec861b3a5e96e349b109308e0dbd0ca6c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:11:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 06:11:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:33:03 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Tue, 07 Jun 2022 06:35:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a9e1b9fcef7c2fa9911bd9f2bf51591102ee0367a667e154cf15f20d0c6faa6a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.15_10.tar.gz';          ;;        armhf|arm)          ESUM='12489d268a6758dc72c073b11a25eb494804649f4760db05b2ef9ddb71aab73e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.15_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd0fad840c3aa118c0ab4cf4070cb9ad25c0ccab456aa22f9b5fc02f4230b26a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.15_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d371ecceccf1d807ca9f0721dba805c65dddc9c5e59c5faaabad37f191970745';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.15_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='22831fd097dfb39e844cb34f42064ff26a0ada9cd13621d7b8bca8e9b9d3a5ee';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.15_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:35:42 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:35:43 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 10:39:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 10:39:04 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 10:39:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 10:39:07 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 10:39:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:39:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:50:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 07 Jun 2022 10:50:13 GMT
ENV TOMCAT_MAJOR=8
# Mon, 13 Jun 2022 21:02:36 GMT
ENV TOMCAT_VERSION=8.5.81
# Mon, 13 Jun 2022 21:02:36 GMT
ENV TOMCAT_SHA512=729387275cce4a0900289722f6c70ebcf7aee924af671b110b8ea8577fd6d045d47f17d526c8db5fd41c8590102e7f5100e95e89f7fd511b941565812ecbed35
# Fri, 22 Jul 2022 02:20:36 GMT
COPY dir:4bb3d085aa9181981607ea878982cba12c5c99e5d382c2a57c71ec8461cbef98 in /usr/local/tomcat 
# Fri, 22 Jul 2022 02:20:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Jul 2022 02:20:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 Jul 2022 02:20:43 GMT
EXPOSE 8080
# Fri, 22 Jul 2022 02:20:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908ba35702b3545e3156e807426eb36d13103c223acf51195f236f759910d212`  
		Last Modified: Tue, 07 Jun 2022 06:23:28 GMT  
		Size: 15.7 MB (15730049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c74d049c5ddc3decb1ebb39938ca716c38ce7d33a45ccbd29d815b3ce60ca9`  
		Last Modified: Tue, 07 Jun 2022 06:43:27 GMT  
		Size: 37.4 MB (37365209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6df4369415b34fa368ddc52bb5b09730a66dff299a2e8780fe53f91d4662f42`  
		Last Modified: Tue, 07 Jun 2022 06:43:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c451aedf74002b88807973b0934b4ffae74f6440f2a78d7d92304d82cff592`  
		Last Modified: Tue, 07 Jun 2022 10:55:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559bd9fee8d200849e2b8491f5934484c9f2fb0592ca69bc3ae50491a1d0519`  
		Last Modified: Fri, 22 Jul 2022 02:35:38 GMT  
		Size: 11.3 MB (11274364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9291060e96ab16ac032ca1d6c2a4eb0d7fefa22f16b5259f6c59cb7120e1c86a`  
		Last Modified: Fri, 22 Jul 2022 02:35:38 GMT  
		Size: 2.1 MB (2051133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57717af56ad8e86b1efee0134ebde941a412e3e3af03de4a36f96fb3c2c69b97`  
		Last Modified: Fri, 22 Jul 2022 02:35:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
