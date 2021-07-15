## `adoptopenjdk:15-jre`

```console
$ docker pull adoptopenjdk@sha256:11be0747a373442d2a7ff144c14439c3af565f24e2eafdd52ed49e09da42dc07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:15-jre` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:b8d99ac0319a8de7547625f3dae846448a333d8c877cd4f572785f1cbd211eb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103115243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225fc173c793285543aafcd1b786d106d555dba35ddaee3e020d185e9bb3e376`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:29:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 00:30:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:31:02 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 00:31:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c1fc968d76004b0be0042027712835dcbe3570a6fc3a208157a4ab6adabbef2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='304be224952dbea7000cda6223b2978b3eefdf2e3749032c3b381a213c8d9c5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dc2480948ac3e6b192fb77c9d37227510f44482e52a330002d6e7497a62a7d67';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='93d81a245f70373a459fe4b1c99c8fb7f357de5c8a14a127f580704270037054';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='31af7efdb1cc0ffd001bc145c3d255266889ad6b502133283ae8bf233d11334c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 00:31:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1182b8c86e6bb404b0d40d2cdcdcaf4347c5aad464143625307b362caff690`  
		Last Modified: Wed, 14 Jul 2021 00:44:02 GMT  
		Size: 16.0 MB (16033076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15c2cf4d362a662bb2b404cf8516825150a4cb6b403e691ba93403806b9fef`  
		Last Modified: Wed, 14 Jul 2021 00:47:09 GMT  
		Size: 58.5 MB (58516304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:7e1b0709f160486837dd9dd11f7c4b6b3eb57c9ef3ad5bcca0c0ea6bdfd37afa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92971042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946f298b71d5f64417746063214cb741eef8c42c574683399ea2441398b8bc71`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:08 GMT
ADD file:1ec1791cf8b61620293d0fdf83d76f3c07482a327aefef699a43e82e7c3aa0f0 in / 
# Tue, 13 Jul 2021 23:21:08 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:28:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 01:29:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:31:05 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 01:31:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c1fc968d76004b0be0042027712835dcbe3570a6fc3a208157a4ab6adabbef2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='304be224952dbea7000cda6223b2978b3eefdf2e3749032c3b381a213c8d9c5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dc2480948ac3e6b192fb77c9d37227510f44482e52a330002d6e7497a62a7d67';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='93d81a245f70373a459fe4b1c99c8fb7f357de5c8a14a127f580704270037054';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='31af7efdb1cc0ffd001bc145c3d255266889ad6b502133283ae8bf233d11334c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 01:31:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:5c5378967b4ed259bac71be5e1a9ea052469b5fe62bed34b19deb57d53dc63c0`  
		Last Modified: Tue, 13 Jul 2021 23:26:18 GMT  
		Size: 24.1 MB (24062066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3374ff0390670de6a897592ab5ae9d7b16efe9170df99397d09cef4f6c91dab4`  
		Last Modified: Wed, 14 Jul 2021 01:36:42 GMT  
		Size: 14.9 MB (14899010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3745f0c31e89f1720bc5faf47bdad301df53d1fd3144d3ed2ad97a7a68a1602`  
		Last Modified: Wed, 14 Jul 2021 01:42:27 GMT  
		Size: 54.0 MB (54009966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:c10b0312ad1601b67a1af199f8adfccedf9faef7a0f7ff52d5a5004dd12d40f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100402180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:390d61b45565969e7b31537667c532311940b20262ba1eba5c95694789b69bb7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:23 GMT
ADD file:4a34ac318ec122d2262279f4f06fd87cdf0383df4b0919cd46f3455b4fcb20a2 in / 
# Tue, 13 Jul 2021 23:01:23 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:20:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 13 Jul 2021 23:20:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:21:34 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 13 Jul 2021 23:21:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c1fc968d76004b0be0042027712835dcbe3570a6fc3a208157a4ab6adabbef2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='304be224952dbea7000cda6223b2978b3eefdf2e3749032c3b381a213c8d9c5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dc2480948ac3e6b192fb77c9d37227510f44482e52a330002d6e7497a62a7d67';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='93d81a245f70373a459fe4b1c99c8fb7f357de5c8a14a127f580704270037054';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='31af7efdb1cc0ffd001bc145c3d255266889ad6b502133283ae8bf233d11334c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 13 Jul 2021 23:21:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:99006dae3b24cf096633c9f0234ddeefee9042d4bede6ebc607d63a52bb79fb0`  
		Last Modified: Tue, 13 Jul 2021 23:03:36 GMT  
		Size: 27.2 MB (27169081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cecec673b168a0ebad3a078ce217e36ce02c414e41ae4f1da4d174e8fdda1b`  
		Last Modified: Tue, 13 Jul 2021 23:24:23 GMT  
		Size: 15.9 MB (15894072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a3bdf91e93434eb1ab6f6313d28a3036875d4f2aff3d2cb2f48ce28ee4ab2`  
		Last Modified: Tue, 13 Jul 2021 23:26:43 GMT  
		Size: 57.3 MB (57339027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:2265587c99d4e48ccae226d844ce98f090d079f2ecdf36a7c14925388394f2a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104860602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3efa825344452bb48f06ff4c849074ac9c04b88d45a57f0ddf43ee53c21e112`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:24 GMT
ADD file:cdca4c00902f291c6bc305420b891f5149b6833b5f9892232ea690d38adfff3f in / 
# Tue, 13 Jul 2021 23:22:32 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 03:31:11 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 14 Jul 2021 03:33:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 03:37:02 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 03:38:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c1fc968d76004b0be0042027712835dcbe3570a6fc3a208157a4ab6adabbef2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='304be224952dbea7000cda6223b2978b3eefdf2e3749032c3b381a213c8d9c5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dc2480948ac3e6b192fb77c9d37227510f44482e52a330002d6e7497a62a7d67';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='93d81a245f70373a459fe4b1c99c8fb7f357de5c8a14a127f580704270037054';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='31af7efdb1cc0ffd001bc145c3d255266889ad6b502133283ae8bf233d11334c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 03:38:51 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:157ef43c951ca9b65226089aef70b09df64b81636884260390a329c24a3c614b`  
		Last Modified: Tue, 13 Jul 2021 23:27:34 GMT  
		Size: 33.3 MB (33287846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604a426cc1c0f74e2a16d10bcce2e153fc2a096f2b79145159b6b14cd92e7c3e`  
		Last Modified: Wed, 14 Jul 2021 03:58:54 GMT  
		Size: 17.2 MB (17208554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bd2cd405b85a3764954d97aa50bf2fcd1eab750e4cbcfa3c03842e89999f76`  
		Last Modified: Wed, 14 Jul 2021 04:01:27 GMT  
		Size: 54.4 MB (54364202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:46dc75474d830fefaaf2558f608d9423dc51539ab7e407bd11a807cfb67316e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.5 MB (95480589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bf2b63952c1ad4dd9fd973beee24529877b34c18cdd8e193c52a107700f60e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:34 GMT
ADD file:ae5354f89d91eedd0614e3e97ee59fd6e23254923062c288d775e19b137dfd1c in / 
# Tue, 13 Jul 2021 22:53:36 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:18:40 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 13 Jul 2021 23:18:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:20:16 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Tue, 13 Jul 2021 23:20:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c1fc968d76004b0be0042027712835dcbe3570a6fc3a208157a4ab6adabbef2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_aarch64_linux_hotspot_15.0.2_7.tar.gz';          ;;        armhf|armv7l)          ESUM='304be224952dbea7000cda6223b2978b3eefdf2e3749032c3b381a213c8d9c5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_arm_linux_hotspot_15.0.2_7.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='dc2480948ac3e6b192fb77c9d37227510f44482e52a330002d6e7497a62a7d67';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_ppc64le_linux_hotspot_15.0.2_7.tar.gz';          ;;        s390x)          ESUM='93d81a245f70373a459fe4b1c99c8fb7f357de5c8a14a127f580704270037054';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_s390x_linux_hotspot_15.0.2_7.tar.gz';          ;;        amd64|x86_64)          ESUM='31af7efdb1cc0ffd001bc145c3d255266889ad6b502133283ae8bf233d11334c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_linux_hotspot_15.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 13 Jul 2021 23:20:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
```

-	Layers:
	-	`sha256:761fa758059faa0c80b0b90fcbcc192fc7f573da055460d5b3f019e0faceeb7a`  
		Last Modified: Tue, 13 Jul 2021 22:55:47 GMT  
		Size: 27.1 MB (27149318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0237838e148d45cea54b0d86c053131b4152f4928836cbb3a0c83ba79b538728`  
		Last Modified: Tue, 13 Jul 2021 23:32:23 GMT  
		Size: 15.7 MB (15741695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d2cdeb83455eceed5c189c312bd098c87ad166436a53ce1ffdc3bb8e01e83`  
		Last Modified: Tue, 13 Jul 2021 23:34:03 GMT  
		Size: 52.6 MB (52589576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:6658de19fe1995bdbec0dc42052f5b59065f604ce8a29246152747cf1fba1dd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2777142518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4541f724490b568fb90817ec209424f49d81ce05a93086018ba78cfe08c869b1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:41:54 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 15:48:27 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_windows_hotspot_15.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_windows_hotspot_15.0.2_7.msi ;     Write-Host ('Verifying sha256 (e78fb1b0ccb6413d27dd9ed487f09af3bd0ba204208305c3b20e58607f45a019) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e78fb1b0ccb6413d27dd9ed487f09af3bd0ba204208305c3b20e58607f45a019') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce6df93f815a40de3f547d56761345861bc8bd00382ec86438652d1e237aa20`  
		Last Modified: Wed, 14 Jul 2021 16:53:10 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fe0777bd9b791c130bedc9602e40d523202145f3112cbddfdae0f7e1ed7884`  
		Last Modified: Wed, 14 Jul 2021 17:01:08 GMT  
		Size: 91.7 MB (91692877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jre` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:e876debc403bed947282fe2559e336f84b96519a0785127506e4adc5a16528e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6361251313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2478d5da8a3d336244138b51c9051f205fa2c7a92ec7a459aeb1036ac04fa2c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:44:07 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 15:50:43 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_windows_hotspot_15.0.2_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jre_x64_windows_hotspot_15.0.2_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (e78fb1b0ccb6413d27dd9ed487f09af3bd0ba204208305c3b20e58607f45a019) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e78fb1b0ccb6413d27dd9ed487f09af3bd0ba204208305c3b20e58607f45a019') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8251f66e6b3e3c9f703ddcda7d3490340fc0c9c6717d3e0aaaa9d1f15811f31a`  
		Last Modified: Wed, 14 Jul 2021 16:53:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a0844b5e16a80b8152dd8a303121e266178a116fdc91ce25d0e32481dbb1ba`  
		Last Modified: Wed, 14 Jul 2021 17:03:10 GMT  
		Size: 91.6 MB (91616549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
