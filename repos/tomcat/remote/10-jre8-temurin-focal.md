## `tomcat:10-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:787e39e9a1fbb27a6497711c788bbc181a6effd5ecbce7ec6324b97105c5f4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:10-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:564dc26af98a8e6b49f4b72d46a0ca1318a9dc676b2277aa17d074275a9a42b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95999649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557b77dcfad73ede4365cce93dd88c3bd2424cba8107157db1dfe3e35eeb81cb`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:19:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:20:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:20:17 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:21:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 11 Aug 2022 19:21:50 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 11 Aug 2022 21:35:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:35:23 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:35:23 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:35:23 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:35:23 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:35:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:35:24 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:35:24 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:35:24 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:35:24 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:35:24 GMT
COPY dir:13ff517c7c38ac369475f1ee0c0dbc31438122076fd2ce00d8fb229e8dd7c492 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:35:29 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:35:30 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:35:30 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:35:30 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aaad0dc3faf013330a30e044ebf8fcfe3d73ac2c342d3879297cd427cf888bc`  
		Last Modified: Thu, 11 Aug 2022 19:30:14 GMT  
		Size: 12.6 MB (12550796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5933f5d2d633d1908a439e66d19af022d468300551349e41c0ff63f5f42c27e9`  
		Last Modified: Thu, 11 Aug 2022 19:31:36 GMT  
		Size: 41.8 MB (41807742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42d5b993bd39daf661f7b050d3e20988fc27f8d222814822f32242d96e58bd9`  
		Last Modified: Thu, 11 Aug 2022 19:31:32 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a058b94eb9848e70fd2b2d9fe13a3a084d48ae946efbee9011bbc9b44d5957`  
		Last Modified: Thu, 11 Aug 2022 22:03:15 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5747eb401867fdd14623212cf169471b270ac8314c428bea8eb6d40d0b7c980a`  
		Last Modified: Thu, 11 Aug 2022 22:03:17 GMT  
		Size: 12.6 MB (12632457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80da15bc16631632a6314ee0d553d3d2e0145acbb5ce0bb0fa8ab042a45d7804`  
		Last Modified: Thu, 11 Aug 2022 22:03:16 GMT  
		Size: 435.6 KB (435595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa04aaa97552cb5dec178da3b4a55765834cd9e8b32bbdd786263fe9db0e696`  
		Last Modified: Thu, 11 Aug 2022 22:03:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:f2883b4a6bf567a8f26bd78f0f483866f29565e85e90021786cf36b92be5b961
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.1 MB (89067002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518d52873a6a8734a7316fcb797f32807f119860f1d85be5369da675d0d5359e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:57:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:57:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:57:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:57:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:57:54 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 18:59:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 11 Aug 2022 18:59:07 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 11 Aug 2022 20:18:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:18:19 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:18:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:18:19 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:18:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:18:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:18:20 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 20:18:20 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 20:18:20 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 20:18:20 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 20:18:21 GMT
COPY dir:bbad8b51c90ce404f364ea3091950194590fe2e00936dc30c3bb01128a6e3b48 in /usr/local/tomcat 
# Thu, 11 Aug 2022 20:18:28 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 20:18:29 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 20:18:29 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 20:18:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a62569004c1e56a6607db95d1fa179d7810f9f0158dc151120981d8941ccdc`  
		Last Modified: Thu, 11 Aug 2022 19:05:37 GMT  
		Size: 12.0 MB (11955821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98894c0c82370f80386dec5a12e5060c9577c044c6a7b1409403e0960306b72c`  
		Last Modified: Thu, 11 Aug 2022 19:06:31 GMT  
		Size: 39.5 MB (39527565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef16899abc5fb5f2bd1921591d19e9e784f5ed5a328d38df6527547ca0ec90bd`  
		Last Modified: Thu, 11 Aug 2022 19:06:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bc22c5cd27ed582b02bf49b128eaf9b3c5e0662a045bd4a09b0e8213bcf3ff`  
		Last Modified: Thu, 11 Aug 2022 20:52:15 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ade306739520a8645e2fec5067875b2a6863bb7dab7aff73a9dc655992cd34`  
		Last Modified: Thu, 11 Aug 2022 20:52:16 GMT  
		Size: 12.6 MB (12582038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389aa61e01f26b81bf369f2bde0c0268ef2034471b4838a9e81b3ec16cd2aec`  
		Last Modified: Thu, 11 Aug 2022 20:52:15 GMT  
		Size: 411.8 KB (411845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4b77191651b91316d00e6291d7c96bc20f9d1fb27361090477815a8f3c164a`  
		Last Modified: Thu, 11 Aug 2022 20:52:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:9d88521c930ba6fcf84457b4eae40311fe5934b8d437060dec13256812b6358d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93252205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d861b4dd7b3bf4886eac0ad3465b8ef8df156a6dae5a39a0d1fcfb15207ea7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:39:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:39:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:39:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:40:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:40:14 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 18:42:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 11 Aug 2022 18:42:03 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 11 Aug 2022 21:06:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:06:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:06:15 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:06:16 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:06:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:06:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:06:19 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:06:20 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:06:21 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:06:22 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:06:24 GMT
COPY dir:c40baef03d09b8b58eeee956b16984783d9bd6dd6842579591ecaddbadd6787b in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:06:30 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:06:32 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:06:33 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:06:34 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedefaaae9298d2004182d1bfde0bea8b977b933e65bb038764a6677dd0632f`  
		Last Modified: Thu, 11 Aug 2022 18:52:30 GMT  
		Size: 12.4 MB (12408927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5efec8a5c172cc90cbdd55b4858b39087bfe6ea907e56bd7f1f3d641bc485c2`  
		Last Modified: Thu, 11 Aug 2022 18:53:43 GMT  
		Size: 40.8 MB (40802933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ce8e05b3c19f22e7ddaea002e59c1d19029e9df2517c32f42e233da466929`  
		Last Modified: Thu, 11 Aug 2022 18:53:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9cd4c1cd84a01027a89e3c95a89acacb982116046cfa4382fe9868ac250f63`  
		Last Modified: Thu, 11 Aug 2022 21:52:13 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eca39fc9f2aaae0774ab74c05d044a7802815934d52afaef0f3396c331e551`  
		Last Modified: Thu, 11 Aug 2022 21:52:15 GMT  
		Size: 12.6 MB (12649541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ef293a42b6b9811ea93f5972eceaa4c794bdee2039bad218b18133fb704ed3`  
		Last Modified: Thu, 11 Aug 2022 21:52:13 GMT  
		Size: 198.7 KB (198732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:197fb22eed072107c24a1652e586e5ae5beeec6f2b14aaae5c7e7bde74feb2e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100706838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da5fed029f407572a1256975c94a1658d3c2e51d883f02e60d2ef90a7a1ab2e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:16:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:16:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:16:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:17:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:17:28 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:20:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 11 Aug 2022 19:20:36 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 11 Aug 2022 21:08:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:08:11 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:08:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:08:14 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:08:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:08:14 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:08:14 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:08:15 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:08:15 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:08:15 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:08:17 GMT
COPY dir:aad8131e71d3bcc530512c81d0182828ff43e846c4245c16d886cf01640e6683 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:08:24 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:08:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:08:27 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:08:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b71b197bc93f31065ddd7245d2113f873ba097b56794545d788a6630da2b0d`  
		Last Modified: Thu, 11 Aug 2022 19:33:13 GMT  
		Size: 13.1 MB (13083533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efe3ab67d35f18000d6b9ccd348c1a1760e9a0b3891fffa3b02e88de84a0ce2`  
		Last Modified: Thu, 11 Aug 2022 19:34:48 GMT  
		Size: 41.2 MB (41194535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82cbf6b919954e7749f500fb64c5e07c54245a9dbccfd657f1cd964cebfcd30`  
		Last Modified: Thu, 11 Aug 2022 19:34:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00403348f6bc05fde294170d98c6a2a9ce6ccd7ad15437fdef26761c21c2317a`  
		Last Modified: Thu, 11 Aug 2022 21:48:02 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed35df7eac0839eb09a9177ae03303ec42de6dd506dee5305999b6b811bbc00a`  
		Last Modified: Thu, 11 Aug 2022 21:48:03 GMT  
		Size: 12.7 MB (12671933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9768c8eb90f242e0c5e4e01bc37c38b80d17a2605c0fd6fed585028479cc0157`  
		Last Modified: Thu, 11 Aug 2022 21:48:02 GMT  
		Size: 461.0 KB (461023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598bdb8b5426043f39acf674c7013cb1b7f69629973de6278a7b13ec20369a8f`  
		Last Modified: Thu, 11 Aug 2022 21:48:02 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
