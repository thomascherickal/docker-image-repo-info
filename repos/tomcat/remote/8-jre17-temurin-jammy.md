## `tomcat:8-jre17-temurin-jammy`

```console
$ docker pull tomcat@sha256:cea925a5360dc49ced397c5e860fbf8ffb9dd85f08dad39614566e008d070cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre17-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:6dd002f864c9ff154778ad3680b4d8a7a30a804ec4b120730694d3977bacf99c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (106045542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a33a21b0d01ea6956a28db6ec42574f8ee07a71652fe945eef91815a83fb5713`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:45:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:45:54 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 01:46:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:46:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 07:42:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 07:42:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:42:02 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 07:42:03 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 07:42:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:42:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:54:52 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 07:54:52 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:05:18 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:05:18 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:05:18 GMT
COPY dir:70d0abc4e6fded56ed75a3a374261580243df58d6e53ec7079e5ead674f16155 in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:05:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:05:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:05:24 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:05:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d923227d8dc300e1ddab1b65c83c0eff7f4a7105d958420872f7138b79735`  
		Last Modified: Fri, 09 Dec 2022 01:52:47 GMT  
		Size: 17.0 MB (16973851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5834fb29a8c053b7e32a51fb2f4174641af50fc2d1edb654decd504eed49f008`  
		Last Modified: Fri, 09 Dec 2022 01:53:37 GMT  
		Size: 47.0 MB (46956958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc10fb884811df88a4d063519deae5ee27e6d20d9a233f74960c3b5cc230c2e`  
		Last Modified: Fri, 09 Dec 2022 01:53:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4db53c47705d84801977f85e57830bd34233d26ad43f0b6a0fc021d773663fe`  
		Last Modified: Fri, 09 Dec 2022 08:04:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e74c11c519761e10ba938b860b392df66cdfa5d4c95f4284f05231e98228d0`  
		Last Modified: Fri, 20 Jan 2023 03:18:15 GMT  
		Size: 11.2 MB (11229800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdf24904804554f0670fe7362bfab17207f462ad0a1c97998cfc7a874ff78bb`  
		Last Modified: Fri, 20 Jan 2023 03:18:14 GMT  
		Size: 455.8 KB (455762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6187dd7395403758b51752cedd6bc20b5406cb21a74ad69923ccfe957d015d`  
		Last Modified: Fri, 20 Jan 2023 03:18:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:1db9c30f3afeff41677ba5527e7aedcf9ef6f337847d7503ad5e8cdfa0ed330d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.2 MB (100210857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f74476972bbce82d7bb3cf69983ebf4bdb82742ddbbdcc9e130c1990e34798`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:36:30 GMT
ADD file:ca82b3c78a23b75345429f192c4b1f88b4e49e12808c85fccc2db04823c17d4e in / 
# Fri, 09 Dec 2022 01:36:30 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:08:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:08:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:08:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:11:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:11:45 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 03:12:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:12:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 04:45:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 04:45:20 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 04:45:20 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 04:45:20 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 04:45:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:45:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 05:01:14 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 05:01:14 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 02:13:58 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 02:13:58 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 02:13:59 GMT
COPY dir:1144dedca8457c422ea851b694ae1e1dc4120504591f01a5caf0c5698eedb488 in /usr/local/tomcat 
# Fri, 20 Jan 2023 02:14:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 02:14:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 02:14:05 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 02:14:05 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c38006c9acc492149d706593acba951110798e57a7ad05103ae7a2d5969c14b6`  
		Last Modified: Thu, 08 Dec 2022 18:49:27 GMT  
		Size: 27.0 MB (27023448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6fead26d897f0226328eb57da4817740f240c9183f841f0c698ed5801d6005`  
		Last Modified: Fri, 09 Dec 2022 03:20:49 GMT  
		Size: 17.1 MB (17093483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8209e965b5937867612c829528fa64b05fa5b3ca3304ecba757a5da1ec78215`  
		Last Modified: Fri, 09 Dec 2022 03:21:48 GMT  
		Size: 44.5 MB (44500308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196fb0c694b720c8fc5b7f113380c1ae42f151c12e35a0ab1d2d0a8e938dec17`  
		Last Modified: Fri, 09 Dec 2022 03:21:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5410bc3aeb6e94b1f53fa2e5465f504691ce0c9c529ae112780de5dff206c3`  
		Last Modified: Fri, 09 Dec 2022 05:19:58 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3404aa3e0aa5f408f08d1ca02bdc004d88ed1bac5dc810f26d8e3c3bbe35b523`  
		Last Modified: Fri, 20 Jan 2023 02:32:34 GMT  
		Size: 11.2 MB (11163433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12639ce2e40f00029a70a4eca488b2897e61cb4257f091dfb0f034145a05a5fa`  
		Last Modified: Fri, 20 Jan 2023 02:32:32 GMT  
		Size: 429.8 KB (429758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d0e4c18b6586965b09c85d6c19d454525346f7b9da68739072309b576ec1c7`  
		Last Modified: Fri, 20 Jan 2023 02:32:32 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:9f3803e7087c5d2ef6e7e52d25a5100b9d5b420f82a0e600f5a52fa2b233b70f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104875717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c1efdc12c7326f6cc853861a5df3b7cc677b47f63c64571aefe8bba301c62`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:39:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:39:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:39:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:42:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:42:00 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 03:42:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:42:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 06:18:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 06:18:56 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:18:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 06:18:57 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 06:18:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:18:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:29:14 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 06:29:14 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:25:13 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:25:13 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:25:13 GMT
COPY dir:dbc89bad979254671000eae9104d9dd0ce68d6e4ceff8fc921e3749bb47d3e2b in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:25:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:25:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:25:18 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:25:18 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f2e5e37e706412c1481b71d2240df4fe659ef83ae4d2932a8ddfe42b0d3d20`  
		Last Modified: Fri, 09 Dec 2022 03:48:04 GMT  
		Size: 18.4 MB (18400373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62df99821b27078a467753cef75400b64ac01ff5752eb0efbc87eaf141f0bb`  
		Last Modified: Fri, 09 Dec 2022 03:48:47 GMT  
		Size: 46.4 MB (46398582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7503a0cabf5d9cf54c23553cd5984a349fcd672e772db22be066516d879a91b`  
		Last Modified: Fri, 09 Dec 2022 03:48:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4158b7a44cffa9be01d8d6467c6034577db5a723a2f72b7aedac87a01777af`  
		Last Modified: Fri, 09 Dec 2022 06:38:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01d079a4416e9ee32c7ff94ada7fd835256938316d0c5169eee00d50c28407e`  
		Last Modified: Fri, 20 Jan 2023 03:37:15 GMT  
		Size: 11.2 MB (11235827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa944bd2419929fdd74aad63da786d02aba8d69da58effeeda8897c2b79aa04`  
		Last Modified: Fri, 20 Jan 2023 03:37:15 GMT  
		Size: 456.0 KB (455999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cac7c0b65e7e829d4743306e14f4ba401adad9c7eb2e267fa5055e60a49c13`  
		Last Modified: Fri, 20 Jan 2023 03:37:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:8a05e2bf8917424afc2d1b95ffbc3f74a3423b817f2ecc08f4f2bf2142e3c5de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112517725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46abdf4883a166f7e78598f22d37e3e2f96111100f95f61ffdd121e1065cd4cb`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:53 GMT
ADD file:1a2557b357a1dca8521ee846ec16c9b2bd8a53839b9d4fda21a28f9ceeecb4b7 in / 
# Fri, 09 Dec 2022 01:27:55 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:39:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 02:39:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 02:39:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 02:45:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:45:22 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 02:46:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 02:46:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 06:52:43 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 06:52:44 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:52:45 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 06:52:46 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 06:52:46 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:52:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:19:15 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 07:19:15 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 03:05:36 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 03:05:36 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 03:05:37 GMT
COPY dir:6d0b3ac675da2e1a0316bc1e2a5c973810f6f1c53d6141007359e7d3e41afa5c in /usr/local/tomcat 
# Fri, 20 Jan 2023 03:05:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 03:05:52 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 03:05:52 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 03:05:53 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ce75b47e476cd75b30dca46558ac79b39923aa94d7e4b0cc025e521404cdbab0`  
		Last Modified: Fri, 09 Dec 2022 01:30:32 GMT  
		Size: 35.7 MB (35708154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b742749281388888fe53f807ad7ae6b5c091713777c43c8f4f21cc50f873d5`  
		Last Modified: Fri, 09 Dec 2022 02:57:27 GMT  
		Size: 18.3 MB (18256829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db881bd5bd28d03dac54043e0ee49b7a0164722792cfd87779973e37e01d066b`  
		Last Modified: Fri, 09 Dec 2022 02:58:44 GMT  
		Size: 46.8 MB (46807534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0f3afeb57ec83faca5edf32e07489d6a10206a9a5c137eb04fde2de1aea4f3`  
		Last Modified: Fri, 09 Dec 2022 02:58:32 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d121ada7fa7fb707da2f7aaf507b3f1d03f6b45de602bb602a457834cfc85e`  
		Last Modified: Fri, 09 Dec 2022 07:38:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e23620ed23d17b16dd11da06d5c5dbc550ad3d17c0b619bd9a04ce3e2c8fbb`  
		Last Modified: Fri, 20 Jan 2023 03:24:47 GMT  
		Size: 11.3 MB (11258035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bd161800af830599790d5e0d8c669ada10353b87d110d7687499a4c157578d`  
		Last Modified: Fri, 20 Jan 2023 03:24:46 GMT  
		Size: 486.7 KB (486709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0418e7e0dbf263144eb349e34c015c8ed5ee0ed2a570369056f2d7a64bd7ce5`  
		Last Modified: Fri, 20 Jan 2023 03:24:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:5b28c5c9e5fed1144bbaee90c1ed655c0af3eaa857dad4be26b73765ea152ff5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100814731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85c77337b6c704a9520be81801abe32b623d390858541be47a3adecbc6a86e70`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 09 Dec 2022 01:52:57 GMT
ADD file:aa22431536efed6cf05ad353979a4d4d5557c975e4333985e7b89b125f013ade in / 
# Fri, 09 Dec 2022 01:53:00 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:13:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 02:13:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 02:13:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 02:17:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:17:17 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 02:18:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 02:18:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 04:35:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 04:35:13 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 04:35:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 04:35:15 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 04:35:15 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:35:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 04:50:08 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 09 Dec 2022 04:50:08 GMT
ENV TOMCAT_MAJOR=8
# Fri, 20 Jan 2023 00:45:31 GMT
ENV TOMCAT_VERSION=8.5.85
# Fri, 20 Jan 2023 00:45:31 GMT
ENV TOMCAT_SHA512=0fc44133aff9e7e31d6dbb4b6e204d33bd0009b6bd089e5f8c8a1f7dfe7c5feff25d7f6404c4a3c5610e0960b5d0198580171212a2636816a23e21799a4c0467
# Fri, 20 Jan 2023 00:45:31 GMT
COPY dir:1dbaf57b6778a181563e32bb74692b27fdf9164d3b424d2de886c9ee6c0690aa in /usr/local/tomcat 
# Fri, 20 Jan 2023 00:45:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Jan 2023 00:45:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 20 Jan 2023 00:45:39 GMT
EXPOSE 8080
# Fri, 20 Jan 2023 00:45:39 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5125256a405e8f68b6edcff30c8e2e9761127daf8628a48134c73f8f45ce631f`  
		Last Modified: Fri, 09 Dec 2022 01:55:10 GMT  
		Size: 28.6 MB (28642146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2cb03cfd1cfc4a8cf03e540f9f3ee0b37424fdbfff1bddb037316f1b65d26a`  
		Last Modified: Fri, 09 Dec 2022 02:25:25 GMT  
		Size: 16.8 MB (16752899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23083f9a1973f68427b02aed8163605337f0569eb08cb9fc0ee8a92e22ea037`  
		Last Modified: Fri, 09 Dec 2022 02:26:08 GMT  
		Size: 43.7 MB (43736850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18606cd1a8d021fbc89bfd67427cfd2f7abe486cf8590b47bac1a872e2e294ec`  
		Last Modified: Fri, 09 Dec 2022 02:26:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e925745e430d78e419d1b13678cf7b74d3d1151c0d3d5fd86089c5b19ed1f7`  
		Last Modified: Fri, 09 Dec 2022 05:00:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99a3bdaa6add0e083d03a72b2415697172f4f5ab7c3e43fdfd2152bca6df797`  
		Last Modified: Fri, 20 Jan 2023 00:56:12 GMT  
		Size: 11.2 MB (11225154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09d76fd226a2db4e49b22a882cf5cea56d3e423814a1f1a425040855e0ff681`  
		Last Modified: Fri, 20 Jan 2023 00:56:12 GMT  
		Size: 457.2 KB (457220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df277196af7cc1598e594e74c4708efc97ac8dfcb476c5eb7840ece167d6d505`  
		Last Modified: Fri, 20 Jan 2023 00:56:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
