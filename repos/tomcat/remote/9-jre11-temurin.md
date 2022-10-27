## `tomcat:9-jre11-temurin`

```console
$ docker pull tomcat@sha256:cde0f425c66607220ce58cf564b9a177d3e0173ee55660fee10eae5a01f5814e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre11-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:dccab6d4f29205fbcf81c2b4349f4c3a9be88ad8e8ce5f9322fc3e7e32eae8b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (102012846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4fd836cd6af1bce3f31f37ae18603209d9a2f6eba611b32eb497c0e9f273b97`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:41 GMT
ADD file:ba96f963bbfd429a0839c40603fdd7829eaca58f20adfa0d15e6beae8244bc08 in / 
# Tue, 25 Oct 2022 01:53:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:27:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 17:27:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 17:27:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:28:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 17:28:59 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Tue, 25 Oct 2022 17:29:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 17:29:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 23:44:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 23:44:21 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 23:44:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 23:44:22 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 23:44:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:44:22 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:52:17 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 23:52:17 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 23:52:17 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 23:52:17 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 23:52:18 GMT
COPY dir:dcff92a27f2d50b1eb220560589edf710336a78b6a89edba1ace73129b7cf16d in /usr/local/tomcat 
# Wed, 26 Oct 2022 23:52:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 23:52:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 23:52:23 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 23:52:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:301a8b74f71f85f3a31e9c7e7fedd5b001ead5bcf895bc2911c1d260e06bd987`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 30.4 MB (30426374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4688df200b56af3e7b12bd48807e851b1a3717379161a295d43dd3184abec55e`  
		Last Modified: Wed, 26 Oct 2022 16:43:13 GMT  
		Size: 12.4 MB (12442357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718682ba85da99179194681dc4f4a79880ef8e04829f70aeddc8e43275506085`  
		Last Modified: Wed, 26 Oct 2022 16:45:30 GMT  
		Size: 46.5 MB (46498610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030909c11444dd48421e92fb65275fccf474ec59fa8530a4fb3cfd9bf36e649`  
		Last Modified: Wed, 26 Oct 2022 16:45:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22bc586e00dcd70b47cf9d79f2eb00512ade1ff0a777bb798602ef75bd2f3f0`  
		Last Modified: Thu, 27 Oct 2022 00:06:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293551d1ea9cf34e154b7baa107ba930a417483190196e459358afe887173769`  
		Last Modified: Thu, 27 Oct 2022 00:12:31 GMT  
		Size: 12.2 MB (12192399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b35b457d2c60567f08d5dd1c41d0a717d722b7893f71c6fc8e270089d9c657e`  
		Last Modified: Thu, 27 Oct 2022 00:12:30 GMT  
		Size: 452.6 KB (452644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f35c608db7b8c968b3d08feda4f5af9873cc8476a93b7184c9bf86ba61dd0ec`  
		Last Modified: Thu, 27 Oct 2022 00:12:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:a59394b35111bd92926e76e65528ebbf4812d920660c43020532837cd7b3d4a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96261508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438e3a3806c3f1663136ef65894ba84b78cc4fab6377fd1cdb9183727aa3ce23`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:30:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 06 Oct 2022 06:30:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 06:30:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 06 Oct 2022 06:30:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:32:22 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Thu, 06 Oct 2022 06:33:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 06 Oct 2022 06:33:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 06:08:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 07 Oct 2022 06:08:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 06:09:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 07 Oct 2022 06:09:00 GMT
WORKDIR /usr/local/tomcat
# Fri, 07 Oct 2022 06:09:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:09:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:21:50 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 07 Oct 2022 06:21:50 GMT
ENV TOMCAT_MAJOR=9
# Sat, 08 Oct 2022 05:47:33 GMT
ENV TOMCAT_VERSION=9.0.68
# Sat, 08 Oct 2022 05:47:33 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Sat, 08 Oct 2022 05:47:34 GMT
COPY dir:dbff5583a9361798f635fe1a7f48fb382d999c9b70fce0d45aab3cf23c63dcf9 in /usr/local/tomcat 
# Sat, 08 Oct 2022 05:47:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 08 Oct 2022 05:47:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 08 Oct 2022 05:47:44 GMT
EXPOSE 8080
# Sat, 08 Oct 2022 05:47:44 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719b6638b27c56e64e5456f9e5ccd262ec6c6ed045d97ce1df9a938b8e0e1822`  
		Last Modified: Thu, 06 Oct 2022 06:39:41 GMT  
		Size: 12.0 MB (12015320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6eaf871645b2228159db42d1e66c86ab9d6c5396bb7b431fddb8c87e3613bca`  
		Last Modified: Thu, 06 Oct 2022 06:42:05 GMT  
		Size: 44.7 MB (44675151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e56a8200988e0a04aab7137c3ee73c486bc6aadc261dfb806873635c56f7af`  
		Last Modified: Thu, 06 Oct 2022 06:41:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cebcb07886a7b6c9fb658650f36f890b51bdc14d613ad3652468dc2e6356fc8`  
		Last Modified: Fri, 07 Oct 2022 06:49:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0f9a9748f5bfb3cd9c98971e8dd21515a636ba935613e01e8a0b96f393919`  
		Last Modified: Sat, 08 Oct 2022 06:06:37 GMT  
		Size: 12.1 MB (12126150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9dcdd6205c103cba286beb15705ec502113e1bc8d15327d1c8ef828073b6f7b`  
		Last Modified: Sat, 08 Oct 2022 06:06:35 GMT  
		Size: 425.8 KB (425792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fcda232143b2d6cb05aefb4db916c271145da54ac46ec36e217c5790e76615`  
		Last Modified: Sat, 08 Oct 2022 06:06:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:86b48a6a8aed36cb902bdd571debb00f6f4bf9f09f54473ad040a90cba19a31c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.3 MB (98260351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03eff9ad381148807faa143e8f07ac82f7e35c3f9d7cd1488c5c2b1f2dacec3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:09:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:10:29 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 26 Oct 2022 01:11:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:11:07 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 17:11:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 17:11:05 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 17:11:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 17:11:05 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 17:11:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:11:06 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:19:37 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 17:19:38 GMT
COPY dir:19b70270aa9cf6d706cd5db112445c59eb2a1298cc73e91aab9918f3461b4435 in /usr/local/tomcat 
# Wed, 26 Oct 2022 17:19:41 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 17:19:42 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 17:19:42 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 17:19:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d33b973dbba18a894c3b9064cedfece84e92985bce6e3be86a5efef3afdea8`  
		Last Modified: Wed, 26 Oct 2022 01:16:34 GMT  
		Size: 12.4 MB (12400371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a6960b661b00d7e89ea4da7f8c5d2b571d0fd35007d448e17a2d178931aa42`  
		Last Modified: Wed, 26 Oct 2022 01:19:26 GMT  
		Size: 44.8 MB (44824650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d046e5da0a7155986a366554538db9c6dc0dc232da3c7371c4a7f8820c766739`  
		Last Modified: Wed, 26 Oct 2022 01:19:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b7e8ec1dfcdbb8e5a9b2d91a66efd6e7890187e39b81ae20b3e7cdcd34fcd`  
		Last Modified: Wed, 26 Oct 2022 17:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4faa8a44e55bcf121db0d88d2c2c46596dead61108d821af57ed2cd29027445`  
		Last Modified: Wed, 26 Oct 2022 17:42:49 GMT  
		Size: 12.2 MB (12200353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c86ceac19f6bc02db83ad0acfe2ab7352de33d019ba1b9c9255ae48cce51489`  
		Last Modified: Wed, 26 Oct 2022 17:42:48 GMT  
		Size: 452.0 KB (452025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1d8957962e1a8cc040e5ae2ae5ae95f438b443ba81a3cf40fa90f1795475c`  
		Last Modified: Wed, 26 Oct 2022 17:42:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:b566c82c41405100810db289f24a6b5c2a54ce966f8c632d774c7737eba19440
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103566062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba1d419acd6958ffbe960feca4fc9b43d1d27392f409f4fe332a13fe01d4ad8`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:47:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:47:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:47:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:47:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:49:30 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Tue, 25 Oct 2022 13:50:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 13:50:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 02:00:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 02:00:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 02:00:36 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 02:00:36 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 02:00:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:00:37 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:15:24 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 02:15:24 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 02:15:24 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 02:15:25 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 02:15:26 GMT
COPY dir:d3d51b68d471a34bbbcc616a9c594e5ee8d2b1da21532a79bd0ca4e46ba4a1fd in /usr/local/tomcat 
# Wed, 26 Oct 2022 02:15:35 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:15:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 02:15:38 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 02:15:38 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b03548b709077a95a1d389c380123c26cac903f8c75f9ad589c4adad13fe9`  
		Last Modified: Tue, 25 Oct 2022 13:58:58 GMT  
		Size: 13.3 MB (13266255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb073ab4820589ed4c8e50a08e7b19dd2173a122e20ab4651121996991e0b4`  
		Last Modified: Tue, 25 Oct 2022 14:02:03 GMT  
		Size: 41.9 MB (41884587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89e904a8b9be59091cb509ff2567906e66b05de59319c2bc1c9e87e728e860e`  
		Last Modified: Tue, 25 Oct 2022 14:01:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b965bd164ccbe7f4237469770c182a641a45fcbdb81b7b6cc48efccba7ac2e85`  
		Last Modified: Wed, 26 Oct 2022 02:41:37 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29de7387f09142344217a4ac310615fd8aaca969b1acca68ac20f88f67e6132d`  
		Last Modified: Wed, 26 Oct 2022 02:49:45 GMT  
		Size: 12.2 MB (12221382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaaea513470b92126a8fbf38af92fd896d31e26bd707550f95062bea2d2e15e`  
		Last Modified: Wed, 26 Oct 2022 02:49:43 GMT  
		Size: 484.0 KB (483975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe868ed3352671ad111fa48a2a7d82dfd808b71848079c77cefcc469a38ef38`  
		Last Modified: Wed, 26 Oct 2022 02:49:43 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:16ff9e75704c1f95214c96fa0a6c23f5c6e3accf4461c87c93ac266ca0268c96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94267956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b311e9c691095ea6c605b4451554f0f3864b996bb5a01eee6756a6745da4ab2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:00:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 09:00:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:00:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 09:00:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:00:51 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Tue, 25 Oct 2022 09:02:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 09:02:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 25 Oct 2022 19:58:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 25 Oct 2022 19:58:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 19:58:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 25 Oct 2022 19:58:55 GMT
WORKDIR /usr/local/tomcat
# Tue, 25 Oct 2022 19:58:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 25 Oct 2022 19:58:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 25 Oct 2022 20:11:07 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 25 Oct 2022 20:11:08 GMT
ENV TOMCAT_MAJOR=9
# Tue, 25 Oct 2022 20:11:08 GMT
ENV TOMCAT_VERSION=9.0.68
# Tue, 25 Oct 2022 20:11:08 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Tue, 25 Oct 2022 20:11:09 GMT
COPY dir:31c14aadc5e199be415fbb62cfe36ba5ec3d55cb4d81fae1c541eb09d30d6186 in /usr/local/tomcat 
# Tue, 25 Oct 2022 20:11:14 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 20:11:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 25 Oct 2022 20:11:15 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 20:11:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c12934f592a5b457e371eff46f533bcd046264666150eb758403450a82ae26a`  
		Last Modified: Tue, 25 Oct 2022 09:11:13 GMT  
		Size: 12.5 MB (12502123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9aeb2eaa0947c0986c8f7acc6ed994c614a42e16397555b3e3138d5068eabf`  
		Last Modified: Tue, 25 Oct 2022 09:11:52 GMT  
		Size: 40.5 MB (40479576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bec7e3375c8ca29206db320122ef01f82c5b3214fe24590cca1b5bec029f9a`  
		Last Modified: Tue, 25 Oct 2022 09:11:46 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdb8c7cebd3e0ddaa0aef19fb9a1e9f7725322c3e105b8940e698860f0931c`  
		Last Modified: Tue, 25 Oct 2022 20:26:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a180e2c7d7ae25f9d5790fdee1d8d2c6ac44890b4041ca7e6dde336ccd9024`  
		Last Modified: Tue, 25 Oct 2022 20:31:00 GMT  
		Size: 12.2 MB (12189852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b7f648dc2ee244bc262d632018d5c15a2d90ae0fe3ea6ed7ad5fd6528bfa6e`  
		Last Modified: Tue, 25 Oct 2022 20:30:59 GMT  
		Size: 454.3 KB (454275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874f47bc8b312c4bf242da11615ec191270aa1af3f7ccb6b0eb8bd8c2d971464`  
		Last Modified: Tue, 25 Oct 2022 20:30:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
