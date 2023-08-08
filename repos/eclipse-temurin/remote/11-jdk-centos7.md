## `eclipse-temurin:11-jdk-centos7`

```console
$ docker pull eclipse-temurin@sha256:afe21da0d559844cb15e73a441f65593499b2c22f21e1d1d133dfccd32d58c34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:11-jdk-centos7` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:11c02cffe7448f82c9ac274af18b2025c4e8b5b2b6abc6cdc2b179e14e593187
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.2 MB (231179395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76d1c29c4c58357f459f3a7143f0d2b31f318652967927097a3a9dc62bb234ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 11 Aug 2022 19:21:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:21:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:21:19 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar     && yum clean all
# Wed, 26 Jul 2023 00:53:42 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Wed, 26 Jul 2023 00:53:49 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 26 Jul 2023 00:53:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:22:29 GMT
COPY file:75f7304d9612805714414928c48b4214e91025809590e620cda7db6b2b5d0176 in / 
# Tue, 08 Aug 2023 19:22:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 19:22:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e946c336ceae859cd4d70967ac63af2f5351aed0dfe146fa12e896157d2c035`  
		Last Modified: Fri, 12 Aug 2022 17:28:51 GMT  
		Size: 13.8 MB (13789720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90534fe9e4b5f21e2196d06da04f53c244ed0e3daca6a8bf8cca5d42b79f30d1`  
		Last Modified: Wed, 26 Jul 2023 00:58:25 GMT  
		Size: 141.3 MB (141291694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7400d8efff1565599b2fb170c2bcd5737539b11b53cc4b4f59d899a3b852f73f`  
		Last Modified: Wed, 26 Jul 2023 00:58:14 GMT  
		Size: 181.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221238ef06aa41419b031b44691fb752fd0dea6e2fbc0dd814f8e8322ef4db59`  
		Last Modified: Tue, 08 Aug 2023 19:29:54 GMT  
		Size: 643.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-centos7` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:4d1fb101cb918b23e809827576fc9921cc231e6029e77f2cc92a3ae0bcf377ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260788423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3a2ea0b69a0b60ec9c53d1c85d1b646adcaef28e8400d59936858b1039ac4e`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Wed, 26 Oct 2022 01:09:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:09:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:09:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:09:36 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar     && yum clean all
# Wed, 26 Jul 2023 00:37:36 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Wed, 26 Jul 2023 00:37:43 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 26 Jul 2023 00:37:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jul 2023 00:37:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7f1658b00328097c595ebc985d4147ed732e13a6abb6228f5db45ea35f873`  
		Last Modified: Wed, 26 Oct 2022 01:16:54 GMT  
		Size: 14.4 MB (14383757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9201f780d8335d02b43e4bc02da2c26f10731363a0ca9617969e825c46021073`  
		Last Modified: Wed, 26 Jul 2023 00:40:24 GMT  
		Size: 138.0 MB (138029544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce7200ed7d0686f4d11e88d75239fee40a1fbc896c7b7a76c55f576e8effa6b`  
		Last Modified: Wed, 26 Jul 2023 00:40:16 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-centos7` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:dc5327b841c69d5b66df7bf3a5ff43ca8bc4904ad676e26da60e82f2bc61e7e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.7 MB (222735852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29017ff037e6b0690086b1e4150d7991ded8268171bf33b3da7905a3a11cdc68`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 15 Sep 2021 18:29:27 GMT
ADD file:7f21ae7d20a8e347d8b678bcf26be83abb1ee27d3b567c9cddd993e45ce8ac34 in / 
# Wed, 15 Sep 2021 18:29:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:29:40 GMT
CMD ["/bin/bash"]
# Thu, 11 Aug 2022 19:19:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:19:39 GMT
RUN yum install -y tzdata openssl curl wget ca-certificates fontconfig gzip tar     && yum clean all
# Wed, 26 Jul 2023 00:17:54 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Wed, 26 Jul 2023 00:18:12 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Wed, 26 Jul 2023 00:18:19 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jul 2023 00:18:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3fe478aaff9b8f3ba958253e7339e9016ec07c075b805ebfc8cd372ddd01ee64`  
		Last Modified: Tue, 17 Nov 2020 04:06:20 GMT  
		Size: 80.5 MB (80516460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0867462d675122ef191a9c60cfd06321372590626128884857fb78457b40b2a5`  
		Last Modified: Fri, 12 Aug 2022 17:33:43 GMT  
		Size: 13.7 MB (13725244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30baff23701aacac336905bca5d3ce1c205aa4822b4ffc5c560f54d0b42fa32d`  
		Last Modified: Wed, 26 Jul 2023 00:23:28 GMT  
		Size: 128.5 MB (128493973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c1775a0785e5b3e6e0badc0d280e568ab088198ed1da89fb6d6625991a77be`  
		Last Modified: Wed, 26 Jul 2023 00:23:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
