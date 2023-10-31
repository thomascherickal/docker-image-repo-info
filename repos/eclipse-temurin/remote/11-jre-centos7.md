## `eclipse-temurin:11-jre-centos7`

```console
$ docker pull eclipse-temurin@sha256:6d986f5d60d631663059a89bca182f76ba3caf51815200be153331f630d70e8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:11-jre-centos7` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:d394fa92f73e133f68503868151463ec0ecb3ceb9cdab64be0ad6b37f31aa88e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135003423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b212869aea84233a575c16a0cbbad4215061220179908784040610dc4cf5e174`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

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
# Mon, 30 Oct 2023 23:25:12 GMT
RUN set -eux;     yum install -y         gzip         tar         curl         wget         tzdata         openssl         ca-certificates         fontconfig     ;     rm -rf /var/cache/yum
# Mon, 30 Oct 2023 23:25:12 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:26:17 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:26:17 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:26:17 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:26:18 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27057586889aa48a720280288d5d3dd8d27075f74b04342230d906fbbdcba6ae`  
		Last Modified: Mon, 30 Oct 2023 23:33:16 GMT  
		Size: 14.8 MB (14831551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae92588f1245cdb1bcd7c338dcf341ede17a3225ea3ab56f9a8c191723b0a91c`  
		Last Modified: Mon, 30 Oct 2023 23:34:52 GMT  
		Size: 44.1 MB (44073844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad527dcd23829437af0d1d3bfd8dc9a3bf09e212c48948f5383991eaad21e3ef`  
		Last Modified: Mon, 30 Oct 2023 23:34:46 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6580c6b6352bba0f52e71cac09291d17be6442fd18b69b9d091c659f68bd0bc`  
		Last Modified: Mon, 30 Oct 2023 23:34:46 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-centos7` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:6473b6ea9c6a4004bbbde85c64d67f1c883c086f0ab8e9ed3ebfe68c864d5f9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.2 MB (165172572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a44b50a1fac2df3cc3e09603d697c4b2a71ed771047b4c18904ef152d23ca17`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

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
# Mon, 30 Oct 2023 23:42:09 GMT
RUN set -eux;     yum install -y         gzip         tar         curl         wget         tzdata         openssl         ca-certificates         fontconfig     ;     rm -rf /var/cache/yum
# Mon, 30 Oct 2023 23:42:09 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:43:06 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:43:07 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:43:07 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:43:07 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f35e75eedae15e1e25c2a47ce5218e22a62b3d69cc35b59c62ef294bf884920`  
		Last Modified: Mon, 30 Oct 2023 23:48:44 GMT  
		Size: 14.4 MB (14389275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43846382ae5f35a64090e31e816c82fade6f58253d2733bc1b0f4ec6be603ede`  
		Last Modified: Mon, 30 Oct 2023 23:49:55 GMT  
		Size: 42.4 MB (42407481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b484a9aece61fd5da8966bfa4d6cdbb7ad08b4ccff86098984ae994e0e9e015`  
		Last Modified: Mon, 30 Oct 2023 23:49:51 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8975675ecdb0639bee59aeb8b693239a25e3f484db98818a507f4f4bd43fb8f`  
		Last Modified: Mon, 30 Oct 2023 23:49:51 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-centos7` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:5446c8ccdab008ac5f56ee637b3a1e84b0ecc7921b9aad0b6ff86d803b8581e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134826794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f1d71411c16a0d7b81f3a38d5dadbc755884956fc41aa9d26d5d0b1e29ae07`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

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
# Mon, 30 Oct 2023 23:20:33 GMT
RUN set -eux;     yum install -y         gzip         tar         curl         wget         tzdata         openssl         ca-certificates         fontconfig     ;     rm -rf /var/cache/yum
# Mon, 30 Oct 2023 23:20:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:22:31 GMT
RUN set -eux;     ARCH="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Mon, 30 Oct 2023 23:22:33 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:22:33 GMT
COPY file:e097c113ce7e2c199bdbde78dd6f9b89c841d973017b0333b39720f0efa4c730 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:22:34 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:3fe478aaff9b8f3ba958253e7339e9016ec07c075b805ebfc8cd372ddd01ee64`  
		Last Modified: Tue, 17 Nov 2020 04:06:20 GMT  
		Size: 80.5 MB (80516460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975b7bd754b874f2dc1cc381b0091e8eab2e8e4b9392a7ab73d4419236699240`  
		Last Modified: Mon, 30 Oct 2023 23:30:23 GMT  
		Size: 14.8 MB (14763841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7792887b6d4e2222f2d71f6c97c5543ed9a9315c5acd099f60d559b516ea26`  
		Last Modified: Mon, 30 Oct 2023 23:31:48 GMT  
		Size: 39.5 MB (39545622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985728c44c3815cefef369c19ab8339623288cc0a010f97cbb922f150453f565`  
		Last Modified: Mon, 30 Oct 2023 23:31:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175e2564d9f3ff24e82f9acfb8d4297278e0116cf0d2e11f224a29a75447e82`  
		Last Modified: Mon, 30 Oct 2023 23:31:42 GMT  
		Size: 711.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
