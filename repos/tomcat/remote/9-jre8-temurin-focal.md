## `tomcat:9-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:a149d8d6f1a771ee12d22e78d35331c974275d41b11c56774829f2d9cb8fab3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:463af83661ab4afb06b15aef8421f7693697a435fa7c92e70f7694aa1a034c16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95617181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08c31fd37e76d84d3638091e3ea4e6556c5c4fc99645e451d480fcd6377ef167`
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
# Thu, 11 Aug 2022 21:40:56 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:40:56 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:40:56 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:40:56 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:40:56 GMT
COPY dir:df1a90f0c6e1dc2b50c81b82e12e88a746378fe5a1366b1c6f1ccda6474c8d74 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:41:01 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:41:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:41:02 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:41:02 GMT
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
	-	`sha256:96bb3383a6c102dfe9c8f171153ea19775b20170bd79417eabd2bca8f93bb27d`  
		Last Modified: Thu, 11 Aug 2022 22:08:35 GMT  
		Size: 12.2 MB (12249994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fb7a7c3da94fbc33724b81495d6e559e88cd7029b721cbef427d1e1eb0e31c`  
		Last Modified: Thu, 11 Aug 2022 22:08:34 GMT  
		Size: 435.6 KB (435590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eb59d723b14906eedc44df6e8830aad06b6e31e6debcff96575caa038aa556`  
		Last Modified: Thu, 11 Aug 2022 22:08:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:7e30dad7d0fd2baf099d55fa744345c6d419c815ce9ffa3e79c752198c210037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88682780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26316e72b392416093dfdfe3198389d757ef668e2ab025ba7cfa289cb472203f`
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
# Thu, 11 Aug 2022 20:25:06 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 20:25:06 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 20:25:06 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 20:25:07 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 20:25:07 GMT
COPY dir:76bcd2966768037f1b1f313a22c91c522fac883144a36541950c584255439aab in /usr/local/tomcat 
# Thu, 11 Aug 2022 20:25:14 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 20:25:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 20:25:15 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 20:25:15 GMT
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
	-	`sha256:920f0d2b85edba90841c206e340d5dbdcb1bb61079620fcae27a8ee6092acafc`  
		Last Modified: Thu, 11 Aug 2022 20:57:52 GMT  
		Size: 12.2 MB (12197842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f239cb3b5be921ad720cff8329f569c7b747ff0f5fd26ccd1cd9f1856a3e26c7`  
		Last Modified: Thu, 11 Aug 2022 20:57:51 GMT  
		Size: 411.8 KB (411818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdc9001f593bda952da32b6872b3c571b17c7bdeca22ee61f6f4d07bf25a610`  
		Last Modified: Thu, 11 Aug 2022 20:57:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:36e3a4c15d425b3863794c3581eca6fe131723f464754ae7cfbd1cfe4fd5de9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92868711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c8733b9518bb26ad2de3cecad4b1f95fb98e313021b7a958f24e8afcba05e77`
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
# Thu, 11 Aug 2022 21:15:42 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:15:43 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:15:44 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:15:45 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:15:47 GMT
COPY dir:3b28d6e44aeeedd13d8b117648c260e07e9d62e835776167110f0f77e348f453 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:15:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:15:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:15:56 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:15:57 GMT
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
	-	`sha256:bb4cc056c9586fab2c4ef61ba8a2cde3a298d3b0d0a0461dbadb86a319ca1a38`  
		Last Modified: Thu, 11 Aug 2022 21:58:43 GMT  
		Size: 12.3 MB (12266037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23892f830654da4b0f0869dad8b357b065b557ba45dacaf808cc8ee33fb4229e`  
		Last Modified: Thu, 11 Aug 2022 21:58:42 GMT  
		Size: 198.7 KB (198742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:5fd0a7a166a18c21c2b6fefe316dfb0f224f16cd408f90ad6687286e3b1ccb3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100326137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c91ae21c841ad5c53be516b3eb7b0fe68bf13903709b4bc6529e16c638f4aad`
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
# Thu, 11 Aug 2022 21:17:36 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 11 Aug 2022 21:17:37 GMT
ENV TOMCAT_MAJOR=9
# Thu, 11 Aug 2022 21:17:37 GMT
ENV TOMCAT_VERSION=9.0.65
# Thu, 11 Aug 2022 21:17:37 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Thu, 11 Aug 2022 21:17:38 GMT
COPY dir:d2ed6ba353083854b068e362d7115f821a2bb421dc6e4e7bf05c39a4c7dd5125 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:17:46 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:17:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:17:49 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:17:49 GMT
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
	-	`sha256:76d0adab677c36ea0f9eb6c1997743475879cf2ec4241753d2f4a8cbd6b59e67`  
		Last Modified: Thu, 11 Aug 2022 21:54:04 GMT  
		Size: 12.3 MB (12291207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ae7666e6c28be61ea95edbb5c02a6f65f1e0fbb6b1b61fc8a35fd1b7bae0b5`  
		Last Modified: Thu, 11 Aug 2022 21:54:03 GMT  
		Size: 461.1 KB (461050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00c143fd7602c6e010734565c607a66768aee6e1e973d66be8c62f86f663cd3`  
		Last Modified: Thu, 11 Aug 2022 21:54:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
