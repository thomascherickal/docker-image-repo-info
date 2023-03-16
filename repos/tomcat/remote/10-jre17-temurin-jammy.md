## `tomcat:10-jre17-temurin-jammy`

```console
$ docker pull tomcat@sha256:88c33f42d030778d9582ec1bc8c706c76ad3e314bf100b68852ca1e60ac25d1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:10-jre17-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:5f4413548356390f5f3682ecec33e1f3873696f471c66bbf12eb22d930ce08ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (107020301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81fe6e9f09861c0db3a4bce54526c14e9c409fd1b8d5fe86270b1087f217b96`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:04:12 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:04:12 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 04:04:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:04:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 10:45:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:45:22 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:45:23 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:45:23 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:45:23 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:45:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:46:08 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 10:46:08 GMT
ENV TOMCAT_MAJOR=10
# Mon, 06 Mar 2023 23:33:34 GMT
ENV TOMCAT_VERSION=10.1.7
# Mon, 06 Mar 2023 23:33:34 GMT
ENV TOMCAT_SHA512=41997f90baf86af6dc0396cbf66941f801e0ae9ad1b57475661d10e648c55559491e85468af2df3ee457be3fcae12b74537ce19a9a28e34030b98e8bb38dbd35
# Mon, 06 Mar 2023 23:33:35 GMT
COPY dir:63c8be519b72da32519cab57fe2fe3b909a7ba6fd4e033925b09bd9753bb3e8b in /usr/local/tomcat 
# Mon, 06 Mar 2023 23:33:39 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Mar 2023 23:33:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 06 Mar 2023 23:33:40 GMT
EXPOSE 8080
# Mon, 06 Mar 2023 23:33:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b1a92356537d7da60fe31ae822ddc345f01a1be49b099c3b7d2bd576ae3b49`  
		Last Modified: Thu, 02 Mar 2023 04:10:40 GMT  
		Size: 17.0 MB (16975272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e504afe67521c2c247b6281da2fd3855688339eee739d255a086542fc67bf1d6`  
		Last Modified: Thu, 02 Mar 2023 04:11:33 GMT  
		Size: 46.9 MB (46935537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c732984ccf01fa98bce820be5b3ec0f48a9a0d85d8b48d190af249202bb8049`  
		Last Modified: Thu, 02 Mar 2023 04:11:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae018c5b2eb1a91463803b9530a94cdb0c9257842d305b70123db83788e98bb`  
		Last Modified: Thu, 02 Mar 2023 11:01:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115c80c832d73f58ec2bd8822021f9cdcbe0ee78dd3fe37a52ef014bfb4494b`  
		Last Modified: Mon, 06 Mar 2023 23:48:55 GMT  
		Size: 12.2 MB (12222095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674c134e2565aeda1bfb7ee119be678b34d82e1b263bc9d04f1056fd5be8fd0a`  
		Last Modified: Mon, 06 Mar 2023 23:48:54 GMT  
		Size: 456.9 KB (456933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d2efe6f32d09a79e7b91130a3b4ebef9e7963627138e413efb444c3ae53ddc`  
		Last Modified: Mon, 06 Mar 2023 23:48:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:1eeb47558c53410f429345c82fbb613a6f15989e848d3b1bc7a4ad45916fe2bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101276653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1701ba009ac8292b8cee8e344382b8371be988b8708816b3a09e026674dda7ae`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:31:41 GMT
ADD file:e9c3ac290fb81ae2e78de99052d776396ee3aff05e1a66fd2dccb01d7de9bb45 in / 
# Wed, 08 Mar 2023 04:31:42 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:46:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:46:15 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:46:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:49:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:49:36 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 02:50:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:50:09 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 16 Mar 2023 04:49:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 04:49:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 04:49:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 04:49:55 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 04:49:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 04:49:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 04:50:41 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 16 Mar 2023 04:50:41 GMT
ENV TOMCAT_MAJOR=10
# Thu, 16 Mar 2023 04:50:41 GMT
ENV TOMCAT_VERSION=10.1.7
# Thu, 16 Mar 2023 04:50:42 GMT
ENV TOMCAT_SHA512=41997f90baf86af6dc0396cbf66941f801e0ae9ad1b57475661d10e648c55559491e85468af2df3ee457be3fcae12b74537ce19a9a28e34030b98e8bb38dbd35
# Thu, 16 Mar 2023 04:50:42 GMT
COPY dir:21e04f36c257a0cb9bea2e25a9c777a1beabc6763a565fd998b77ccbff94c537 in /usr/local/tomcat 
# Thu, 16 Mar 2023 04:50:46 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:50:47 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 16 Mar 2023 04:50:47 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 04:50:47 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cba1fa3bcdf4f746dcf5b8f86874cee4a6eff75dd5c5cd29e4c912574b12a1c6`  
		Last Modified: Thu, 09 Mar 2023 04:41:14 GMT  
		Size: 27.0 MB (27025397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85169cff2ee4bc04fcfaf94a937435e69eb27ca38bf1dcbd04593cccacf0d702`  
		Last Modified: Thu, 16 Mar 2023 02:56:32 GMT  
		Size: 17.1 MB (17093778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be72bd479c96978965e7a3ad3512673e6ca3b26714713ca967a807e2c0bcdb7e`  
		Last Modified: Thu, 16 Mar 2023 02:57:28 GMT  
		Size: 44.5 MB (44528811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5725cdfe807b737e733d3d3a443ffd37aef0141ba7a33fb98b334c479486085`  
		Last Modified: Thu, 16 Mar 2023 02:57:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4387aaa79ab90896ad19499f9700bb569a1cf1c15ffc0fa6052dec8ea82f0707`  
		Last Modified: Thu, 16 Mar 2023 05:10:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792e3bc1d6153b0d45c148870e6a1642d0d054521b80fced311e371b77647f61`  
		Last Modified: Thu, 16 Mar 2023 05:12:22 GMT  
		Size: 12.2 MB (12197555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24933cd908b8635669b6e668bcfc160f8832ddc45429737ff0f18d3af6da412`  
		Last Modified: Thu, 16 Mar 2023 05:12:21 GMT  
		Size: 430.7 KB (430655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaa7508bd33f1ae525a0a027c69bb50b5bbe20ef17793804f75e3c4c4d6d93f`  
		Last Modified: Thu, 16 Mar 2023 05:12:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:79ca9a793c2f085182794a5df4b6f4676fe6a1a3255fe45538c9b05e71170004
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105889275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e332a26986a35efd4675a3b88c1ab28b94a9e002ad96433c37cbcaec86fc4637`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:55:04 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 16 Mar 2023 01:55:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:55:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 16 Mar 2023 06:26:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 06:26:15 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 06:26:15 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 06:26:15 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 06:26:15 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:26:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:26:51 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 16 Mar 2023 06:26:51 GMT
ENV TOMCAT_MAJOR=10
# Thu, 16 Mar 2023 06:26:51 GMT
ENV TOMCAT_VERSION=10.1.7
# Thu, 16 Mar 2023 06:26:51 GMT
ENV TOMCAT_SHA512=41997f90baf86af6dc0396cbf66941f801e0ae9ad1b57475661d10e648c55559491e85468af2df3ee457be3fcae12b74537ce19a9a28e34030b98e8bb38dbd35
# Thu, 16 Mar 2023 06:26:51 GMT
COPY dir:b1a76aa5fe3903a3955dd7036e9b549e7e0baeebfb2f9fdb7f70ccdf6fe63ad5 in /usr/local/tomcat 
# Thu, 16 Mar 2023 06:26:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:26:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 16 Mar 2023 06:26:56 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:26:56 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dd5efa5ce73b25dc0236fcd408527b63e42c87e6da9672a356731004b8949`  
		Last Modified: Thu, 16 Mar 2023 02:01:25 GMT  
		Size: 46.4 MB (46421360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce9280353ea6c4511dc5378e2f0f4742d499bf6df15c8d10804513c8c5115a`  
		Last Modified: Thu, 16 Mar 2023 02:01:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22574da6a8f30964c321cccc4b118c72ce4409bbe3ed89ecaeb57dde841e1b86`  
		Last Modified: Thu, 16 Mar 2023 06:40:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee78975aa36c32a8faa9150c1720a31b0886a4e3b35e6d6bd097b1b3ca2ad8d7`  
		Last Modified: Thu, 16 Mar 2023 06:41:11 GMT  
		Size: 12.2 MB (12223392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ad9ef39000ec968d18b8d2811bab74cf2aa1b4a382642c0a7de21c15756f9a`  
		Last Modified: Thu, 16 Mar 2023 06:41:10 GMT  
		Size: 455.7 KB (455719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3994bf78dbabc20fc5be0c00c74301d65a93b123ab401c501dc32ef5841233c`  
		Last Modified: Thu, 16 Mar 2023 06:41:10 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:60716b79b704515a2f751b8c872c46a81478cf22eec16d099e9ac508fa060470
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113475264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed168fa6fec5d979fa88efd1347640b40811f7be114b94d8b725236aa0c6d885`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:04:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:04:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:10:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:10:43 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 04:12:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:12:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 06:31:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 06:31:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 06:31:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 06:31:17 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 06:31:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:31:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:33:55 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 06:33:55 GMT
ENV TOMCAT_MAJOR=10
# Mon, 06 Mar 2023 23:45:15 GMT
ENV TOMCAT_VERSION=10.1.7
# Mon, 06 Mar 2023 23:45:15 GMT
ENV TOMCAT_SHA512=41997f90baf86af6dc0396cbf66941f801e0ae9ad1b57475661d10e648c55559491e85468af2df3ee457be3fcae12b74537ce19a9a28e34030b98e8bb38dbd35
# Mon, 06 Mar 2023 23:45:16 GMT
COPY dir:9e63ffd5458ab889e210e71a8da6e00a0ad95fc68a800b45b358d42fc1843353 in /usr/local/tomcat 
# Mon, 06 Mar 2023 23:45:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Mar 2023 23:45:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 06 Mar 2023 23:45:28 GMT
EXPOSE 8080
# Mon, 06 Mar 2023 23:45:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6285377bd773c7b29d366adba27fcbd8df16cebdc3aa9aaa4bec6c3fdf6f91e5`  
		Last Modified: Thu, 02 Mar 2023 04:21:56 GMT  
		Size: 18.3 MB (18257678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f65ad9a7690fb5ed5e91ed728b5f141ef3d3b97678ebcef3970c50818dfd2bb`  
		Last Modified: Thu, 02 Mar 2023 04:23:07 GMT  
		Size: 46.8 MB (46780994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fbb0d715aa698759ab490956accad6caf4c50cc36ae0be0a74ec99aae44e4`  
		Last Modified: Thu, 02 Mar 2023 04:22:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168602f6e3339a0cac138353dc726d45d61e5c22566d81f4d1ed578bf23f3f70`  
		Last Modified: Thu, 02 Mar 2023 07:19:55 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd7709b16b51314af9579ecca3413d83a5d7d3351a0512cbdceb080c3c18dd6`  
		Last Modified: Tue, 07 Mar 2023 00:10:22 GMT  
		Size: 12.2 MB (12236353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d871d99bf430dcdb1eaef4070e9c983b1696594165cc4c7dbab446e1acf6b0ac`  
		Last Modified: Tue, 07 Mar 2023 00:10:21 GMT  
		Size: 488.2 KB (488186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05545e48c3d6d40e60a65632df3e16a8e48603fd1f8f77ee54341390913da6bd`  
		Last Modified: Tue, 07 Mar 2023 00:10:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:1e6584cabb18d6dfb2ca44a80ccc16885f2b2c3e059b394fddcfe00c044b2ec7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101824592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23c37aec3591c9a0cb6b871f0ad84e73bd5ff00188062145f915e10e8599944`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:10:39 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:10:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:10:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:41 GMT
ADD file:db14dc9a9d330115a6699be3c4a344f5fe366ec17e7d3649c4ecb2711605e52b in / 
# Wed, 01 Mar 2023 05:10:41 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 02:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 02:26:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 02:26:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 02:29:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:29:01 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Thu, 02 Mar 2023 02:29:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3797815cb853616b6415e1b8875cda4eaa004887561ea4ea2090d726b8d8582f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='bf7ef7ba477dc278f913e64174e76be9ae7f014c767352eae83b3f9581494fce';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f11b86bfd7fa4d7a0d05040ea235102296f03eaf064253f76d7ab94baa0352e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='21a7156a29e7921bc7c6eadecb8ee4ac7161921cea85b75b61f0376f9c725caa';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='fe669935609086e76cb0b829e92808766cbf8cb7bda57a76b47813b08584bfd2';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jre_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 02:29:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 18:51:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 18:51:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 18:51:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 18:51:32 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 18:51:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 18:51:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 18:52:45 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 02 Mar 2023 18:52:45 GMT
ENV TOMCAT_MAJOR=10
# Tue, 07 Mar 2023 00:25:09 GMT
ENV TOMCAT_VERSION=10.1.7
# Tue, 07 Mar 2023 00:25:09 GMT
ENV TOMCAT_SHA512=41997f90baf86af6dc0396cbf66941f801e0ae9ad1b57475661d10e648c55559491e85468af2df3ee457be3fcae12b74537ce19a9a28e34030b98e8bb38dbd35
# Tue, 07 Mar 2023 00:25:10 GMT
COPY dir:8dc015120b6542e36f88b5cdfae51a9131685d3f95268aa5aeecfdea0858fb0b in /usr/local/tomcat 
# Tue, 07 Mar 2023 00:25:13 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Mar 2023 00:25:14 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 07 Mar 2023 00:25:14 GMT
EXPOSE 8080
# Tue, 07 Mar 2023 00:25:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:905ef75a23211c85ea45c3aa7f7e77bc95a94ff8c250e03412ef8c50b5fb9f49`  
		Last Modified: Thu, 02 Mar 2023 02:23:13 GMT  
		Size: 28.6 MB (28647596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4e01bae29df25fb7bfcdd33039913cef559e9f560e229a4d06ba7d0cf487b6`  
		Last Modified: Thu, 02 Mar 2023 02:35:04 GMT  
		Size: 16.8 MB (16753277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30a580085c8966a9a0029c4d387ac22d878a04ce250fda114387901fb07e837`  
		Last Modified: Thu, 02 Mar 2023 02:35:45 GMT  
		Size: 43.7 MB (43738873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d42063ce60f7ec2fb0037ce0ab82302323f9234a1ea6ce33a491061c75e97c`  
		Last Modified: Thu, 02 Mar 2023 02:35:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552be455cdb990d49149e1c0db992e6fe679bc00c8ea9f042694504b3e73f044`  
		Last Modified: Thu, 02 Mar 2023 19:10:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910f13ba28d4926f408c14214bf951ecf09eeb5545189cee9bca1100a29bee16`  
		Last Modified: Tue, 07 Mar 2023 00:36:18 GMT  
		Size: 12.2 MB (12225885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042a3ba82c7abe1e7e74572edeb50f1ffd957eede178fb7400949401358bc8cc`  
		Last Modified: Tue, 07 Mar 2023 00:36:18 GMT  
		Size: 458.5 KB (458502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3dc69e766a93f30d195008b3fd2bff8fa93c60ad63477116d4cade916f2b9f`  
		Last Modified: Tue, 07 Mar 2023 00:36:17 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
