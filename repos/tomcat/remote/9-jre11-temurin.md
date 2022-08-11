## `tomcat:9-jre11-temurin`

```console
$ docker pull tomcat@sha256:e3a15ad3fe4ae8c75cf0f54651414a00186db0c9253156d626c6e48521bc0a3c
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
$ docker pull tomcat@sha256:3f72534a520b1795390844af28c60db9ab740baa783499f6fcd3ca82c902ab53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100898422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6002a64282280e3f321e4888fec14180ee202563e841148ffdca16a59b4d3fb2`
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
# Thu, 11 Aug 2022 19:20:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:22:41 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:23:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:23:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 21:29:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:29:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:29:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:29:55 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:29:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:29:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:38:09 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:38:09 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:38:09 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:38:10 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:38:10 GMT
COPY dir:2872a1408d58310a889ac08cd5e127119e4a613d5a1ff35128b8eadbcbabbb26 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:38:14 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:38:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:38:15 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:38:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc15e118841a9f177bca811667e37fe099192eb26678de7c0b49e003dac8576`  
		Last Modified: Thu, 11 Aug 2022 19:30:35 GMT  
		Size: 11.3 MB (11343716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06f199c59dc441d577e8ab717f37deca9b48cfdc989034d6483f2fe8baba7b6`  
		Last Modified: Thu, 11 Aug 2022 19:34:43 GMT  
		Size: 46.5 MB (46496410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db1234d90fb8b714eefb18b0a15fbc0f884f6a81af2f4b88123710936a0e23c`  
		Last Modified: Thu, 11 Aug 2022 19:34:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeade929514a0cf9b1fa62731ba3a0ab5a74e93af51b4d413764e477404db75`  
		Last Modified: Thu, 11 Aug 2022 21:56:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70505b37cdcb668ca467688721c959210b64e8e0b21aac4d199734cf478136c2`  
		Last Modified: Thu, 11 Aug 2022 22:06:03 GMT  
		Size: 12.2 MB (12185001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4213bbbf38cbe4ba3ba4dceeb1793e559804b9902671edae0da1d8febc101770`  
		Last Modified: Thu, 11 Aug 2022 22:06:02 GMT  
		Size: 446.7 KB (446696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d09d794e3b6613e19eae40b13e1cc4d96cbdcddc29b66c232206c3c9bce098a`  
		Last Modified: Thu, 11 Aug 2022 22:06:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:6add338210d7529e70371c1a7e99d2c012056dd5f4b62a08f20d311263163eaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95296353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328c32930fac133f1ae8d91722cdc7b6a2f7e341ade581d9b79e6881ee5d836c`
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
# Thu, 11 Aug 2022 18:58:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:59:53 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:00:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:00:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:11:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:11:04 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:11:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:11:05 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:11:05 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:11:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:21:41 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 20:21:41 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 20:21:41 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 20:21:41 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 20:21:42 GMT
COPY dir:05c048b5e215be31bca741a3e68d2b887b0e950e1b96d4c0e72e2d2ff903e5e1 in /usr/local/tomcat 
# Thu, 11 Aug 2022 20:21:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 20:21:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 20:21:51 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 20:21:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1a5cf9a21e485b0a676c22ced0e80a140055b3ef0d7573caf5be408a10ddb04`  
		Last Modified: Tue, 02 Aug 2022 01:43:32 GMT  
		Size: 27.0 MB (27017015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f83bb11050bc1d50de6dd12d2a1425bd7a5069761fb12910fc0066805ccc5c`  
		Last Modified: Thu, 11 Aug 2022 19:06:03 GMT  
		Size: 11.1 MB (11064474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18824beaf598bf76f3f7f146820fb7773ed45f52eb9d6929099f4d5bcadf306b`  
		Last Modified: Thu, 11 Aug 2022 19:08:28 GMT  
		Size: 44.7 MB (44674533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7b15edaa54f78e477be0a8e1c50b26839e7f1ac451936d5060ebe0fb39e15c`  
		Last Modified: Thu, 11 Aug 2022 19:08:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9383955b6dfc918b48b616d3940e2187f88f45837c9db11adfe9a3be93b3c0e`  
		Last Modified: Thu, 11 Aug 2022 20:44:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb9626ffbfea6b0e5202b3ceb9ec7401b963b877405f9bb1a6fe1ab91501062`  
		Last Modified: Thu, 11 Aug 2022 20:55:10 GMT  
		Size: 12.1 MB (12119316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92c75a653b4a041471ce72a1f16000aec80318e5d25e0d3ec2df7ef54e75e04`  
		Last Modified: Thu, 11 Aug 2022 20:55:09 GMT  
		Size: 420.6 KB (420554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dcce9231a3efe009d86f6c99e1e724e4ae8185807142abe27603edbd0ac5146`  
		Last Modified: Thu, 11 Aug 2022 20:55:09 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:0a73e64616745cde590e04ae87de0ff4f32c7ec14d381d7d32d8bcc6ccd97687
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96920926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a0912dafe001a9c3f4211d9f1f97f9024d3708823537db61f6ee7b172c681f0`
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
# Thu, 11 Aug 2022 18:40:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:43:19 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:44:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:44:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:56:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:56:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:56:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:56:43 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:56:44 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:56:45 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:11:06 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:11:06 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:11:07 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:11:08 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:11:10 GMT
COPY dir:cc091db17cfbdc17f46d1b9507f54f2706538ecd1d2209706f04106a63cffaf1 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:11:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:11:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:11:19 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:11:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b941860b1b56dff93374f7988debb6b45635d744ea5fe506bdc3aff09ba84e11`  
		Last Modified: Thu, 11 Aug 2022 18:52:53 GMT  
		Size: 11.3 MB (11311183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124239d433fcf63e89f26b2341c275998389a5c98e7e35f74756dcfb50eac04`  
		Last Modified: Thu, 11 Aug 2022 18:56:22 GMT  
		Size: 44.8 MB (44827851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dce0813d8cba43018a0f51356f18e76650d59618a1901ca29c80ed4029f546`  
		Last Modified: Thu, 11 Aug 2022 18:56:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d390143210909030afe77603d328db3fbbefea5a8302afff166bd5473ec917`  
		Last Modified: Thu, 11 Aug 2022 21:44:34 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddff00dc2ffbf6ba6568008c6dce9f53279f9302c1a9ec80c0b268f7a05db64`  
		Last Modified: Thu, 11 Aug 2022 21:55:38 GMT  
		Size: 12.2 MB (12191470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965949ff0c6cf5272369b647f5572fcefc2ab9d5e0f24a6edd8e76cdbec895ca`  
		Last Modified: Thu, 11 Aug 2022 21:55:38 GMT  
		Size: 209.0 KB (208968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:28957c734bd85c5016f6942075e99f3b9e969dd269f923cce3d67abbb9f1a85a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102170591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:568b4e9de60c1479adee0248475c916de53c35789c562ff556e7805b0cdbeba9`
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
# Thu, 11 Aug 2022 19:18:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:21:42 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:23:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:23:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:57:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:57:58 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:57:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:58:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:58:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:58:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:12:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:12:55 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:12:55 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:12:55 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:12:56 GMT
COPY dir:8a39bae5402a23be259963b140f3845d863ece5d2164bec3617acba70bc8b4aa in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:13:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:13:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:13:07 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:13:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1beca851dc26aa06b8642a7de984d251e67d42f6e7104fcad4eab7d1664f2090`  
		Last Modified: Thu, 11 Aug 2022 19:33:42 GMT  
		Size: 11.9 MB (11875147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d9ea429dab9dc0d6aa3a4e4cb2dfcdc46cd3d674174c47a131dc84a64c5cc`  
		Last Modified: Thu, 11 Aug 2022 19:38:05 GMT  
		Size: 41.9 MB (41885516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf81efed18b64e0203c1da113af51f07bc3db6caed60cde624d200a0632740`  
		Last Modified: Thu, 11 Aug 2022 19:37:55 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3fc64f72d1695d348e60d5d15ed2420e3abed87f2d7cc4c1fd0e9188ed109a`  
		Last Modified: Thu, 11 Aug 2022 21:40:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a4fa2023e033b6c134e4a4928fdb32ccb7838d2fe68ab83c1abcdb5b5c457`  
		Last Modified: Thu, 11 Aug 2022 21:51:13 GMT  
		Size: 12.2 MB (12213538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a26bbbd7d0af25fa927733c24f0121bbe0f1150e7c7e3df3b0e9c27fa415c4e`  
		Last Modified: Thu, 11 Aug 2022 21:51:12 GMT  
		Size: 477.9 KB (477922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7615ba927cbc25617d80709b21b97fd1ebc5c19b99da3ba0a042723e5a4089bf`  
		Last Modified: Thu, 11 Aug 2022 21:51:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:29b4de85abb489544d1b5e7044c28fbe1b54d1898db0765bf549b8a410b23680
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93166270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76d6d4ba95b264709334fcd38d1d2cab609c3afb4c055d8d607db33762cb4bd8`
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
# Thu, 11 Aug 2022 18:42:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:42:36 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:43:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:43:18 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 19:45:09 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 19:45:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:45:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 19:45:11 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 19:45:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:45:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:57:38 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 19:57:39 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 19:57:39 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 19:57:39 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 19:57:39 GMT
COPY dir:c8433f4be4540813b8d2bd77ecb599bdab87ad07192e3eedca91431310677c36 in /usr/local/tomcat 
# Thu, 11 Aug 2022 19:57:44 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:57:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 19:57:46 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 19:57:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739633e842cf87e58170d8e9c3754c3a3a79b50ed6fd03fa65bbaf2dabcde04`  
		Last Modified: Thu, 11 Aug 2022 18:49:41 GMT  
		Size: 11.4 MB (11412494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d546e934e4fbaa88de69ad2d7df9404d12c4c8e0226f64d693d88e545080bc95`  
		Last Modified: Thu, 11 Aug 2022 18:50:22 GMT  
		Size: 40.5 MB (40479895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c836e0958febc49e5be83535c64cd2d7df8def1e2c92c9b6a5168776283199f`  
		Last Modified: Thu, 11 Aug 2022 18:50:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0a1106f9df170174fd35269f6ff96298121e9232a161b4a35b36768f521b3`  
		Last Modified: Thu, 11 Aug 2022 20:12:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434804058a4c4dd42ab89486d36e6cd7086fab0267bf2081b3ce6700d07789c5`  
		Last Modified: Thu, 11 Aug 2022 20:18:06 GMT  
		Size: 12.2 MB (12182476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfaffaad86bb92403d931674efd8aa0a770f87c34e52011cb1fbc67cac7f62`  
		Last Modified: Thu, 11 Aug 2022 20:18:06 GMT  
		Size: 448.2 KB (448156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7d83b3ea663d1b8ec80a1649881fe80a6bae3f64c7a592d960003b1a68947f`  
		Last Modified: Thu, 11 Aug 2022 20:18:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
