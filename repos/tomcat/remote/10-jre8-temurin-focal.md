## `tomcat:10-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:6353b5cf05a612273d56c78a821131a2f28c5aad4ded2ff47fb88f91deeb140f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:10-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:1d951e12d8481550086fff2c43fec20da71cdec6865e33b7f9ba44774ed84628
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108171999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f91384490892f4a11aaf1d4ec805f2b9a62d6d28f551a5f6c146101f293e1598`
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
# Thu, 03 Mar 2022 21:23:53 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Thu, 03 Mar 2022 21:24:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 21:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:24:11 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 04 Mar 2022 02:38:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:38:05 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:38:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:38:06 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:38:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:38:06 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:38:06 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 02:38:06 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 02:38:06 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 02:38:06 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 02:38:07 GMT
COPY dir:f6fb065fed38ff492bdf14312227eac00e6f1c7daaa8d51d91f4a0f5ff05b558 in /usr/local/tomcat 
# Fri, 04 Mar 2022 02:38:11 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:38:12 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 02:38:13 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 02:38:13 GMT
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
	-	`sha256:ba08f9b93cd6d43e071c9fbf9ec6a3e6ca6376d7f98abe22d23adb809342c368`  
		Last Modified: Thu, 03 Mar 2022 21:27:48 GMT  
		Size: 41.8 MB (41773813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f16eed7419c36b1c92aa1b29f642a58296017a6b23ec2217a46fc44ea1798e`  
		Last Modified: Thu, 03 Mar 2022 21:27:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaaafe11645479f4368643ea74f0c735ed71f11e123b8867e8ac1023482dbd6`  
		Last Modified: Fri, 04 Mar 2022 03:03:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbab135c8266cb4c0dfb2cdbea5568641e87f9bd8c3d770a7bf14778f469e71`  
		Last Modified: Fri, 04 Mar 2022 03:03:30 GMT  
		Size: 12.6 MB (12564879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf788736f50a613253e05e2f90dc1c0874ca39ce52e64d1e8b31bf8d97f7b814`  
		Last Modified: Fri, 04 Mar 2022 03:03:28 GMT  
		Size: 452.0 KB (451983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58421ccd7a7f60b4a364fd745cefc00a8a0f606b9d16288fc87b57e2d948bdcf`  
		Last Modified: Fri, 04 Mar 2022 03:03:28 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:92be091dc4134b814cf937173aea0c33ae7715d65e97f5e64033e3898d1764ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99605232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847f9d9a9348e1b1ed2cd3047f810925896bff137b1a106fe9594110d2eb1903`
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
# Fri, 04 Mar 2022 04:41:30 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Fri, 04 Mar 2022 04:42:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 04 Mar 2022 04:42:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 04:42:31 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 04 Mar 2022 08:56:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 08:56:58 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 08:57:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 08:57:00 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 08:57:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 08:57:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 08:57:01 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 08:57:02 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 08:57:02 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 08:57:03 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 08:57:05 GMT
COPY dir:ad53d6660b54b25d4a98b804c883c1fbff7215acbc7cb88b3a6edb2077855d70 in /usr/local/tomcat 
# Fri, 04 Mar 2022 08:57:15 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 08:57:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 08:57:19 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 08:57:19 GMT
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
	-	`sha256:05325d7388562ba9410d2812621591778474bc4d30f904f6ea3f31bf5fa859df`  
		Last Modified: Fri, 04 Mar 2022 04:50:10 GMT  
		Size: 39.5 MB (39514108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e265cbd85ee89cb10dfbb564d9720f5f1c8b4a3b05997f6c94b2e5728f500b`  
		Last Modified: Fri, 04 Mar 2022 04:49:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49678aa0e85db93b328134588b846054f0c5e0454ac692974ed4b902971b4970`  
		Last Modified: Fri, 04 Mar 2022 09:34:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54299408fa34029a8fc0b256c309bb276d964d830108a014477b72812b1682c`  
		Last Modified: Fri, 04 Mar 2022 09:34:15 GMT  
		Size: 12.5 MB (12513347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf89efe69e90c2275e26aed4498714ed6943986a950e03f249986ecc6aa6af`  
		Last Modified: Fri, 04 Mar 2022 09:34:10 GMT  
		Size: 429.6 KB (429592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72acab7b159f26c95b490892f98cccdeecbbe6432633079b2ef20d10b320067f`  
		Last Modified: Fri, 04 Mar 2022 09:34:10 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:3d3cf4feb188c1f27979862c9e543dd451c309b35f4ddeaefd8d4a1fc8551196
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105499517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9dce813246e81671750915f131447dbd328f5dfd89d9413b48296c40f5ef`
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
# Thu, 03 Mar 2022 20:21:24 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Thu, 03 Mar 2022 20:21:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:21:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:21:54 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 03 Mar 2022 23:45:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 03 Mar 2022 23:45:58 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 23:45:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 03 Mar 2022 23:46:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 03 Mar 2022 23:46:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:46:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:46:03 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 03 Mar 2022 23:46:04 GMT
ENV TOMCAT_MAJOR=10
# Thu, 03 Mar 2022 23:46:05 GMT
ENV TOMCAT_VERSION=10.0.17
# Thu, 03 Mar 2022 23:46:06 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Thu, 03 Mar 2022 23:46:08 GMT
COPY dir:d7c2ebddc01ec1e16ef356a034c1fbf17ccdd234f79c3ffb7218ce51f9c602bc in /usr/local/tomcat 
# Thu, 03 Mar 2022 23:46:15 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 23:46:16 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 03 Mar 2022 23:46:17 GMT
EXPOSE 8080
# Thu, 03 Mar 2022 23:46:18 GMT
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
	-	`sha256:381848042d31ba382c04ec804d9f20abe809e824312bda89997565a6c9a87975`  
		Last Modified: Thu, 03 Mar 2022 20:26:23 GMT  
		Size: 40.8 MB (40769838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308f692c7991588d6b942ca8dc53ab429f9f2453966a72f606099eb7d3a881e8`  
		Last Modified: Thu, 03 Mar 2022 20:26:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c45d760253294a5e88f7c6456194e2e15df04b042d5843d3d492db6256b71e`  
		Last Modified: Fri, 04 Mar 2022 00:37:21 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c7101d54ff3f5dbdffa71551bd35aec6be3bcf57941189d2f89f1afd2fe5ca`  
		Last Modified: Fri, 04 Mar 2022 00:37:22 GMT  
		Size: 12.6 MB (12581208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e5acfbc2c54aa322b6661e188738c6498fc472efbfa038ad188239a515d15f`  
		Last Modified: Fri, 04 Mar 2022 00:37:21 GMT  
		Size: 214.7 KB (214698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:2622f337e0228f78af72d27aabedd9247c44a34575f246d70b2d9f225dee971c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.2 MB (114185511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1e45fc949e2680995ef2397dfb055297f651611ae0b610a80017bebe3e9298`
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
# Thu, 03 Mar 2022 22:06:48 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Thu, 03 Mar 2022 22:07:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='22496d5e677aaccc5a85e90584d0a012c51a08898f0e09e259eabe67ed81da2b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='48181f17b85a13c0e2f260c8f4b39483e61664cf07ea00e6210a666fb5210492';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f15b536a97c27d114c0b59c86de07ca80a271d3979ed0aa056318ea329e31e5d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9c4607cee01919a21c57a36e8c009a7aca7aefd63010c64d7a3023fe8590ebe1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 22:07:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:08:04 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 04 Mar 2022 02:49:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:49:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:49:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:49:53 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:49:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:49:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:50:03 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 02:50:06 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 02:50:08 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 02:50:10 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 02:50:13 GMT
COPY dir:0f2628a4cb589d4ab7d87e497703c5b555e91e2c26829a7856e6d0cdc6845a6e in /usr/local/tomcat 
# Fri, 04 Mar 2022 02:50:35 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 02:50:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 02:50:59 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 02:51:01 GMT
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
	-	`sha256:5d9aa9f46f0e6c25c7880e2665a0ed0b255ab8aa3d1d4a05352399ae35969e66`  
		Last Modified: Thu, 03 Mar 2022 22:17:17 GMT  
		Size: 41.2 MB (41162302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e363b868aaf2dc43d6adb569b2e0031736f84279f493b630e5f6cb0a6b79f579`  
		Last Modified: Thu, 03 Mar 2022 22:17:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599c6100a1974fd1743e17d6529869ce1e2a3a81aadda3c0cc2d03bcd9897ea`  
		Last Modified: Fri, 04 Mar 2022 03:51:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9884b2012205bc5730e8c8fa949006aedba5b85bae474d45632e1bc5aabbf41b`  
		Last Modified: Fri, 04 Mar 2022 03:51:14 GMT  
		Size: 12.6 MB (12607569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8231a487004795fdd57d2f8b868e515ccfdc7f34180458af8cc5110a0815b9aa`  
		Last Modified: Fri, 04 Mar 2022 03:51:12 GMT  
		Size: 477.5 KB (477537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf328d0c74ab4c11fe6736bde2fdb370ce6e562039ac22132ca26a395c8b5d3`  
		Last Modified: Fri, 04 Mar 2022 03:51:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
