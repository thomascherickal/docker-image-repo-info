## `tomcat:8-jre8-temurin-jammy`

```console
$ docker pull tomcat@sha256:533c91d18e638f05504442ce221337f76cb80da85573edecb75ed17eee374eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:8-jre8-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:a5fc5708259bf8432c99f7acee12741b94c403992f949ad25292bfdf8ae7142e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96344027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0858e79d683b4c5b5819180b37357d55e6bf3d5bd73f294c1e59d7d849e992ae`
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
# Fri, 12 Aug 2022 17:20:49 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Fri, 12 Aug 2022 17:21:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 12 Aug 2022 17:21:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 12 Aug 2022 20:19:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 20:19:24 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 20:19:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 20:19:24 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 20:19:25 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 20:19:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 20:30:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 20:30:20 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:34:34 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:34:34 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:34:35 GMT
COPY dir:53ecb0f9152fe86a64bf4a2e605ce345d5086f3097428fb6a70dc46c2fbe7c01 in /usr/local/tomcat 
# Wed, 17 Aug 2022 21:34:39 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 21:34:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:34:41 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:34:41 GMT
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
	-	`sha256:ffc343c126abdd02617e79385eba15e9ceaecee236c68853f15e658e216488bc`  
		Last Modified: Fri, 12 Aug 2022 17:29:31 GMT  
		Size: 41.8 MB (41807941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b80be9c827d6ea5c217fde6b16ccd571715686bc0f912d17c43cb04b8c8d2`  
		Last Modified: Fri, 12 Aug 2022 17:29:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ce7ecd4d7e253a46a795c29a2d7c8743c57a2f1ad7ee7dd2fd986f08484b9d`  
		Last Modified: Fri, 12 Aug 2022 20:46:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1133092c2f108e82ba5504b802e1f40b96f9edce9b43f06ee85b194906d8d3`  
		Last Modified: Wed, 17 Aug 2022 21:56:24 GMT  
		Size: 11.2 MB (11201359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4c2b3b0abf5346844c3230b66621ae2e0d7516f19e45f1e5e6be19b18d6cd9`  
		Last Modified: Wed, 17 Aug 2022 21:56:23 GMT  
		Size: 452.1 KB (452125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683cf962623771221b2604196e99f4b996219316301ec23a21499e20d70719c6`  
		Last Modified: Wed, 17 Aug 2022 21:56:23 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:95d4cf3b218878423e654897e30dafed5421c6d0fd0696cb332c998fbefff8bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90150760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6461e99a025c8c18b4f1292c346ad79ef4681614946fdeffc97dd5ccb4954deb`
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
# Fri, 12 Aug 2022 16:58:35 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Fri, 12 Aug 2022 16:59:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 12 Aug 2022 16:59:21 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 12 Aug 2022 18:22:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 18:22:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 18:22:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 18:22:38 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 18:22:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:22:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:36:02 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 18:36:02 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:08:55 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:08:55 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:08:56 GMT
COPY dir:48db5d6e07e5d7d3c365cb79729d5b01e16a2e6fc6d436bec4443289e3b2e753 in /usr/local/tomcat 
# Wed, 17 Aug 2022 21:09:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 21:09:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:09:05 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:09:05 GMT
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
	-	`sha256:e9d686389641521336b5535b5d5e191d4e45af0fccd7959b9dacc3e44005ae26`  
		Last Modified: Fri, 12 Aug 2022 17:07:16 GMT  
		Size: 39.5 MB (39538004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1397eb5b3263f1bed3217e7427425c7bb692784f9f0b7a729ce28b0f23715548`  
		Last Modified: Fri, 12 Aug 2022 17:07:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4211453a9f8afc77a8fa060d281ca63443bb29c9758c9e23676c39385c207b0a`  
		Last Modified: Fri, 12 Aug 2022 18:56:04 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4326316334a1d651fcabedcb5ff6b085b2bfc9c4938f5691c7af2c47ae3bae8`  
		Last Modified: Wed, 17 Aug 2022 21:28:02 GMT  
		Size: 11.1 MB (11134349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a810d5390cc1706991e97d1b4a0e1453226796bef5dcab2538f758b7e8b78c7`  
		Last Modified: Wed, 17 Aug 2022 21:28:00 GMT  
		Size: 427.0 KB (426987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cc1bddcda997729b8d96ee27a3944aa70ef1abf5acc8b22e9017bafe22807e`  
		Last Modified: Wed, 17 Aug 2022 21:28:00 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:7969fcadad224b614b704aa5545cf2fc66fe9fba70a611d155f435dd97055a99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93020589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de08e0470458a254e565ccc1e9f5e741fdfda5eef0df03a9f51205832f3bcb6`
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
# Fri, 12 Aug 2022 17:40:47 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Fri, 12 Aug 2022 17:41:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 12 Aug 2022 17:41:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 12 Aug 2022 21:25:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 21:25:22 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 21:25:23 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 21:25:24 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 21:25:25 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 21:25:26 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 21:44:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 21:44:21 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 22:09:04 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 22:09:04 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 22:09:06 GMT
COPY dir:8711e90a76245f386b05ca47231264f0e3b7bf24bfefb3234882fbf9b82ec5c3 in /usr/local/tomcat 
# Wed, 17 Aug 2022 22:09:13 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 22:09:14 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 22:09:15 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 22:09:16 GMT
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
	-	`sha256:7405b3c3309315fe08c73916bc088302fb1529509cfa869aa9a9b1b20c4c6e7b`  
		Last Modified: Fri, 12 Aug 2022 17:52:37 GMT  
		Size: 40.8 MB (40803100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53e0b6a8b74408dffbb16486e3e235c8873c63a3d9435cb274bf09b5738805a`  
		Last Modified: Fri, 12 Aug 2022 17:52:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ec5181428693352b13e2b56d9f2d7796327cd20b41c710adba99af11301ffd`  
		Last Modified: Fri, 12 Aug 2022 22:11:26 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58763f899a3aa4c96a8aeb7066d92e24a886fa4f79788e6685dca1a3a7739e5e`  
		Last Modified: Wed, 17 Aug 2022 22:51:08 GMT  
		Size: 11.2 MB (11207295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95829cf9f3afdd2fa8998643c671ebce53dd6dc63d0d538b83298b8e3041132`  
		Last Modified: Wed, 17 Aug 2022 22:51:08 GMT  
		Size: 214.4 KB (214422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:7f80ac94f1219f0ac2b842c86d568e4ac57eab1a0aa1d004a0b8f6bfaaabb460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101908922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f773997df92515d553d82f7a5a2472bdcd186cd73afe9135ff5482b8a9154f99`
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
# Fri, 12 Aug 2022 17:18:29 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Fri, 12 Aug 2022 17:20:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 12 Aug 2022 17:20:24 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 12 Aug 2022 18:40:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 12 Aug 2022 18:40:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Aug 2022 18:40:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 12 Aug 2022 18:40:32 GMT
WORKDIR /usr/local/tomcat
# Fri, 12 Aug 2022 18:40:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:40:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 12 Aug 2022 18:58:47 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 12 Aug 2022 18:58:47 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:31:22 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:31:23 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:31:24 GMT
COPY dir:a8d92eec5b1d61eb85a9f5d60cd0a09d5452561298ae2ac1e6cea65782de2860 in /usr/local/tomcat 
# Wed, 17 Aug 2022 21:31:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 21:31:34 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:31:34 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:31:35 GMT
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
	-	`sha256:0202f5c6f5720470eedc2c0531f45f48d3ff7e81d97b9545ff87bdbf401428eb`  
		Last Modified: Fri, 12 Aug 2022 17:34:38 GMT  
		Size: 41.2 MB (41194804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf96c6b843266451f1bb74c3907be19b76beb05aeaf72ef43493efd16347c96`  
		Last Modified: Fri, 12 Aug 2022 17:34:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac299825b4978ad9560e7dbdf18e25eb1219a3d4a42105c55c0c9d3182a79ba`  
		Last Modified: Fri, 12 Aug 2022 19:19:00 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babc9ba1156a9e4a642a0dafb74bed19e9f5925544ebf68731ebcb4ef4563a70`  
		Last Modified: Wed, 17 Aug 2022 21:49:41 GMT  
		Size: 11.2 MB (11228780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774bda2453a42a4865adba9a4e9bf18fbc87062b27e42bfe42ef2d4c4ea4a45a`  
		Last Modified: Wed, 17 Aug 2022 21:49:40 GMT  
		Size: 483.4 KB (483424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e253cb1983b37f08f0b2111468973b4683d52270ca70fd54228ddfa8e7a6f25`  
		Last Modified: Wed, 17 Aug 2022 21:49:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
