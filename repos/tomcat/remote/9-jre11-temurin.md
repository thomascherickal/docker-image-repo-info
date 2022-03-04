## `tomcat:9-jre11-temurin`

```console
$ docker pull tomcat@sha256:7b574e733b691766fc9c46d9c0c3474fc8e4bd262b8919937f43ea92536d24e9
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
$ docker pull tomcat@sha256:81cbdccc367301ca9f33d4f0c78b4f5feaf486a8d14ecf606678c310340ae956
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109275653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6d0a68c769dd59cb9fa47775e6f36ec7bf9e31684a64c55a77f16ac45e5eb6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 21:23:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:24:18 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 03 Mar 2022 21:24:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 21:24:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:24:40 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 04 Mar 2022 02:33:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:33:10 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:33:11 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:33:11 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:33:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:33:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:42:01 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Mar 2022 02:42:01 GMT
ENV TOMCAT_MAJOR=9
# Fri, 04 Mar 2022 02:42:01 GMT
ENV TOMCAT_VERSION=9.0.59
# Fri, 04 Mar 2022 02:42:01 GMT
ENV TOMCAT_SHA512=74902b522abda04afb2be24d7410d4d93966d20fd07dde8f03bb281cdc714866f648babe1ff1ae85d663774779235f1cb9d701d5ce8884052f1f5efca7b62c68
# Fri, 04 Mar 2022 02:42:02 GMT
COPY dir:90de26adde61af6f02e0893db9493635679d16dddbd6414cca7aa57592afef9c in /usr/local/tomcat 
# Fri, 04 Mar 2022 02:42:06 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:42:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 02:42:07 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 02:42:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60db36418686552d08825174a47afb44becb668d28541be579fb31c0108b0ac2`  
		Last Modified: Thu, 03 Mar 2022 21:27:24 GMT  
		Size: 24.8 MB (24815110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8e34f3db4144e3ecfe1aed2a7a388c2418a9b5598da083ea980a19385c5804`  
		Last Modified: Thu, 03 Mar 2022 21:28:36 GMT  
		Size: 43.2 MB (43230147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d2739dcb2d2ec8fc549a012c8da2587b7659dcb338d668941ec4bbe91acbac`  
		Last Modified: Thu, 03 Mar 2022 21:28:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ed785d19f6d3a957b13df4675feb309802faf5cc601a6562e86942f5eca7ac`  
		Last Modified: Fri, 04 Mar 2022 02:59:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6debbcfb8140a9693785103693a448f3705744c6d202f799f3d75fc7a126c825`  
		Last Modified: Fri, 04 Mar 2022 03:05:52 GMT  
		Size: 12.2 MB (12212189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bbe666863f3ab0f71156c25b980496e52e1df08def14ba361b6ad20a49cf9c`  
		Last Modified: Fri, 04 Mar 2022 03:05:51 GMT  
		Size: 452.0 KB (451993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3c47015c956dbc94e5d81eacb742411877711c65d746e1f555556d8a841192`  
		Last Modified: Fri, 04 Mar 2022 03:05:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:c1cde5ca858c2c74e35674a38f8badc79e308a73bbcc212488f0cac29ad08f05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101586815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1e1b45b1e38de24dfb2dfcac9f9c10f41b7cc49764b065e6e855b29ec7975`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 21:21:31 GMT
ADD file:984d3d8b31abd025bb9be52f42d60245a76b1ee991f286db819ae204da45390c in / 
# Thu, 03 Mar 2022 21:21:32 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 04:40:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 04 Mar 2022 04:41:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 04:42:45 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Fri, 04 Mar 2022 04:43:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 04 Mar 2022 04:43:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 04:43:36 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 04 Mar 2022 08:48:36 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 08:48:36 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 08:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 08:48:38 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 08:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 08:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 09:03:21 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Mar 2022 09:03:21 GMT
ENV TOMCAT_MAJOR=9
# Fri, 04 Mar 2022 09:03:22 GMT
ENV TOMCAT_VERSION=9.0.59
# Fri, 04 Mar 2022 09:03:22 GMT
ENV TOMCAT_SHA512=74902b522abda04afb2be24d7410d4d93966d20fd07dde8f03bb281cdc714866f648babe1ff1ae85d663774779235f1cb9d701d5ce8884052f1f5efca7b62c68
# Fri, 04 Mar 2022 09:03:25 GMT
COPY dir:d977c82e801308fb49340af3e0db956a8f4852fd36736a760a58a34f9a331333 in /usr/local/tomcat 
# Fri, 04 Mar 2022 09:03:35 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 09:03:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 09:03:39 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 09:03:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:12a77aaceb8aa1438ebb61cb4904d74fc225cfa20464a060980580674a0a31e9`  
		Last Modified: Thu, 03 Mar 2022 21:25:09 GMT  
		Size: 24.1 MB (24073718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d5e13fa89bbe7488660a017213f436309a11623cb2fc7e50bcebd3b67b1214`  
		Last Modified: Fri, 04 Mar 2022 04:49:08 GMT  
		Size: 23.1 MB (23074002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aa942fc198abfce250f92ef2e56f89fec27a3a8fe15099886bca113a19f120`  
		Last Modified: Fri, 04 Mar 2022 04:52:19 GMT  
		Size: 41.9 MB (41850611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c5642b7f0d53fd3b7ba8384e571a4229334a9691a54b37e88b0725a4e7d57b`  
		Last Modified: Fri, 04 Mar 2022 04:51:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e603a2f1c5004d24e9bdfe44849fe8732b66410749459f38bb4c630cf0225d4d`  
		Last Modified: Fri, 04 Mar 2022 09:29:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0a881336c38328a29dc38007c288a6bf180ad9311753a6427b778afc9399d7`  
		Last Modified: Fri, 04 Mar 2022 09:37:18 GMT  
		Size: 12.2 MB (12159464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b6b6da412dccba1ee4087ef406d0a14a8f3469e6ef915b5a58a1f3bb240c91`  
		Last Modified: Fri, 04 Mar 2022 09:37:14 GMT  
		Size: 428.6 KB (428557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fedb8ec5961974aa8df906a8ac12b4a1705e5360ac4f1e49b7cf56bececfbcf`  
		Last Modified: Fri, 04 Mar 2022 09:37:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:2bcdd81e50ace12798e3438de0af2b6a233a45080052f2726ea2146652fed370
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105950134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25b96f19ae26a77b941d76cec21702d3071fe81c9e822a1ca8aee7d6079a0b74`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:02 GMT
ADD file:f2fffe739729839aa17484bc4d79d33425549c5052824eac12131b16c23565d3 in / 
# Thu, 03 Mar 2022 19:41:03 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 20:21:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:22:04 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 03 Mar 2022 20:22:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:22:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:22:37 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 23:37:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 03 Mar 2022 23:37:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 23:37:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 03 Mar 2022 23:37:09 GMT
WORKDIR /usr/local/tomcat
# Thu, 03 Mar 2022 23:37:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:37:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:54:00 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 03 Mar 2022 23:54:01 GMT
ENV TOMCAT_MAJOR=9
# Thu, 03 Mar 2022 23:54:02 GMT
ENV TOMCAT_VERSION=9.0.59
# Thu, 03 Mar 2022 23:54:03 GMT
ENV TOMCAT_SHA512=74902b522abda04afb2be24d7410d4d93966d20fd07dde8f03bb281cdc714866f648babe1ff1ae85d663774779235f1cb9d701d5ce8884052f1f5efca7b62c68
# Thu, 03 Mar 2022 23:54:05 GMT
COPY dir:48917acca9070e57deee829365828d5232f04aa234b3522f979e4f6815e2fcfe in /usr/local/tomcat 
# Thu, 03 Mar 2022 23:54:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 23:54:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 03 Mar 2022 23:54:14 GMT
EXPOSE 8080
# Thu, 03 Mar 2022 23:54:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5a7855fb0d7ae372c824d9c76be5ad2f42ce178c1910fa54a8543036b5325fd5`  
		Last Modified: Thu, 03 Mar 2022 19:42:38 GMT  
		Size: 27.2 MB (27169631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa00815a7c2cf918ad429621769d62801eb12468697f2d994bb52711822fed7`  
		Last Modified: Thu, 03 Mar 2022 20:25:54 GMT  
		Size: 24.8 MB (24763878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e544c081bb9267cae02eef16e8b87b1472b2cdb43e003e419c9aece5c0457509`  
		Last Modified: Thu, 03 Mar 2022 20:27:17 GMT  
		Size: 41.6 MB (41572370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c18dc1e49eaa3403f722274d1adbf6ff8d6ad5d7a5758ee618ec2a3b3eed23a`  
		Last Modified: Thu, 03 Mar 2022 20:27:10 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3267b20f75b3c8432c137bf2e9a2fbbcdba7ad6b6008b93d950d259ff9b7d911`  
		Last Modified: Fri, 04 Mar 2022 00:31:05 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849375b8e5f12bd6b4b6850a9d98e441d8035efac46ce9a8f2d0fe0f48995609`  
		Last Modified: Fri, 04 Mar 2022 02:20:44 GMT  
		Size: 12.2 MB (12229292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47869a9f96e8ae94aa246a28e19afe043f189608af22a7deaadc5c4c2615016a`  
		Last Modified: Fri, 04 Mar 2022 02:20:43 GMT  
		Size: 214.7 KB (214697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:83f45844d97bc5c0b8639cb271a020166d7b19fb3a3c60e8fba7fc8952fccde5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111311991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2974e8426de36fe112703af13687fb6be75711401a62dff24edbb3a73c63b7b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:04:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 22:06:43 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:08:20 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 03 Mar 2022 22:09:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 22:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:09:33 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Fri, 04 Mar 2022 02:31:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:31:04 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:31:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:31:24 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:31:29 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:31:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 03:07:11 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Mar 2022 03:07:17 GMT
ENV TOMCAT_MAJOR=9
# Fri, 04 Mar 2022 03:07:20 GMT
ENV TOMCAT_VERSION=9.0.59
# Fri, 04 Mar 2022 03:07:23 GMT
ENV TOMCAT_SHA512=74902b522abda04afb2be24d7410d4d93966d20fd07dde8f03bb281cdc714866f648babe1ff1ae85d663774779235f1cb9d701d5ce8884052f1f5efca7b62c68
# Fri, 04 Mar 2022 03:07:26 GMT
COPY dir:fba152484657d78a4d8eb4600c19ce8696b9634e6530e3df5269a6a6f8525254 in /usr/local/tomcat 
# Fri, 04 Mar 2022 03:07:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 03:08:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 03:08:06 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 03:08:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5899f11433955d19db6d812785121cdffebdc19933e71ca549ee5ed6a7c1696`  
		Last Modified: Thu, 03 Mar 2022 22:16:45 GMT  
		Size: 26.6 MB (26645446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacd6cca57b62a80267ff6d4adbd2f67aa78079cc5781c2775d570c5eb1db7eb`  
		Last Modified: Thu, 03 Mar 2022 22:18:17 GMT  
		Size: 38.6 MB (38640567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3077630d499d05fc4ae3b0638d48658a5a90fd6794214eecce6ec6e66be9b3`  
		Last Modified: Thu, 03 Mar 2022 22:18:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad52f9acd8603e85ae5b6abd2639abd17218cd12e22aa4a5e56daf6505596427`  
		Last Modified: Fri, 04 Mar 2022 03:47:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c3fe697248b1eb64fec5f90ff64b3eda117a69645b524420de4636746a0f71`  
		Last Modified: Fri, 04 Mar 2022 03:53:49 GMT  
		Size: 12.3 MB (12255764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178803ce305ba0505876260a6aaa12d8a20d6ac789c2b0619861613428e657`  
		Last Modified: Fri, 04 Mar 2022 03:53:47 GMT  
		Size: 477.6 KB (477558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c0d254e36c2b5098db3fa2d96cd65d11b0d3c08928a5c8e65387fe0d0e16a1`  
		Last Modified: Fri, 04 Mar 2022 03:53:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:65ccd2a129b93b00ff3cda782400a2e3066156954979ca2c45caef4c7ef58905
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101540035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a9fef3a6e6e560603aecc607b35109cf83d8cbd4bcc18162a1b6dabead86195`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:52 GMT
ADD file:3162233da685a36a9f274a7fa1d99452cab76f37e3640d38851c782ca506f75b in / 
# Thu, 03 Mar 2022 19:41:53 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 19:59:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 19:59:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 19:59:34 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 03 Mar 2022 19:59:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6426ce7dfdacaa798ec7779e0bec30ec8510df491fb2c965e8e6bf2f88af27e9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='964a5d3c1f63209e5ad908a302220b3ba2e81a6574b7b7a5020f736e1496835f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8c9efc13680f43b742a54ecb3be614efd62749d401e780143fef3ac5403a6284';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6b2f0292b5cf9db9ff73bbd75cb0500ec03b3dc10c95c0c8e287a95648ce7785';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b5a6960bc6bb0b1a967e307f908ea9b06ad7adbbd9df0b8954ab51374faa8a98';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 19:59:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 19:59:59 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 21:12:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 03 Mar 2022 21:12:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:12:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 03 Mar 2022 21:12:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 03 Mar 2022 21:12:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 21:12:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 21:20:21 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 03 Mar 2022 21:20:21 GMT
ENV TOMCAT_MAJOR=9
# Thu, 03 Mar 2022 21:20:21 GMT
ENV TOMCAT_VERSION=9.0.59
# Thu, 03 Mar 2022 21:20:21 GMT
ENV TOMCAT_SHA512=74902b522abda04afb2be24d7410d4d93966d20fd07dde8f03bb281cdc714866f648babe1ff1ae85d663774779235f1cb9d701d5ce8884052f1f5efca7b62c68
# Thu, 03 Mar 2022 21:20:21 GMT
COPY dir:9e2de1b14bddba74c0dcfebb5ed0da0bd7befa3a328095fc647e045707aab524 in /usr/local/tomcat 
# Thu, 03 Mar 2022 21:20:26 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:20:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 03 Mar 2022 21:20:27 GMT
EXPOSE 8080
# Thu, 03 Mar 2022 21:20:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ade7e68f4e34f438527a34c9761a285c3c3864e3daab0544b2c4f4163c7c3f56`  
		Last Modified: Thu, 03 Mar 2022 19:43:22 GMT  
		Size: 27.1 MB (27084671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df41031a9799d7c10edff78f849659fc6e07dd869aa06a62a8e4a1b9548dc13f`  
		Last Modified: Thu, 03 Mar 2022 20:02:15 GMT  
		Size: 24.4 MB (24447191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925bee56d3d2d89399385f73319b61fdcd59e5b31d8ef29c57e8212ee0b76b54`  
		Last Modified: Thu, 03 Mar 2022 20:02:37 GMT  
		Size: 37.3 MB (37328942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e85f779153f7b61361387152cc128d46e17850e8292f9edad3ce0043e508eb4`  
		Last Modified: Thu, 03 Mar 2022 20:02:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeae163890f01fbdd279e699c9f1c915ba834b8cebe3f8f8de4e22ea7461343`  
		Last Modified: Thu, 03 Mar 2022 21:30:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80304afed6ebd3e4aa8c2158d9ab2cb0bedbe55e9896c2dd4a330fe40e2d7f87`  
		Last Modified: Thu, 03 Mar 2022 21:33:56 GMT  
		Size: 12.2 MB (12225003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077d6f92c9043fffcb5005c7ea7677b226b8f87f5e8fd99c454e76994c01e063`  
		Last Modified: Thu, 03 Mar 2022 21:33:55 GMT  
		Size: 453.8 KB (453767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a70f4c38108ee27f045c6e2e5e4cd1f7a93e9229f4cc44d42f5fb34e8b5404`  
		Last Modified: Thu, 03 Mar 2022 21:33:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
