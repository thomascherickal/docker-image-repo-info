## `adoptopenjdk:16-jre-hotspot`

```console
$ docker pull adoptopenjdk@sha256:e98133719d363818e06d47a8bbb25bc94a3fe3104897672a8fbfba550cab8931
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

### `adoptopenjdk:16-jre-hotspot` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:acc99f88a18a9954da4f9605c715d907c41fe5648e270ed0f77c2a0459f55931
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94220458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1940a41f74e89777012349a02635e556ee50f413e96bb12e085b9a7bf93d1afd`
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
# Wed, 14 Jul 2021 00:31:54 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 00:32:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 00:32:15 GMT
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
	-	`sha256:895d64beca9665a47ca188cd66b0f1964f8a4952a1903a4a3fb5ca59d7073947`  
		Last Modified: Wed, 14 Jul 2021 00:48:22 GMT  
		Size: 49.6 MB (49621519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - linux; arm variant v7

```console
$ docker pull adoptopenjdk@sha256:ecdc5790c99e36a25dc4ac499f782b384585b23e433882989f66fbecd35ee0c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83624322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99a69193d121218ef17f4a53feafef41a19e27c6875134e7a9166cba2187d77`
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
# Wed, 14 Jul 2021 01:32:13 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 01:33:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 01:33:08 GMT
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
	-	`sha256:4bae0a3905362e257606c5d7b942ac938ceadf184e88921905aaca2aaa16fd9e`  
		Last Modified: Wed, 14 Jul 2021 01:44:50 GMT  
		Size: 44.7 MB (44663246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - linux; arm64 variant v8

```console
$ docker pull adoptopenjdk@sha256:b0124ce287c1441300f349af1f5fe77ec86b980fcdd1fc6cc82b03a55cc14c57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91485749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaf98a43c8a4eec2daec3e89caad62235ebf3a0a719f92e938642d0f98fabea`
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
# Tue, 13 Jul 2021 23:22:04 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Tue, 13 Jul 2021 23:22:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 13 Jul 2021 23:22:32 GMT
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
	-	`sha256:bdfc18f3d0be70c3934a1eec44d4a229e817ef7abc0e5646ef2e3a2fb5666320`  
		Last Modified: Tue, 13 Jul 2021 23:27:44 GMT  
		Size: 48.4 MB (48422596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - linux; ppc64le

```console
$ docker pull adoptopenjdk@sha256:62d640bc846111d2b482a21c74c893b06b5d7e7ef85578980f03381b38eb2e21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95348575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b8059dc2392eb6513363f0d1e5e261543e88f3fe8b64d553da7d634bb5b854`
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
# Wed, 14 Jul 2021 03:39:08 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 03:40:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 14 Jul 2021 03:40:36 GMT
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
	-	`sha256:c81d37e315f3fdb06f6e55d9d770bfc5ff609ccee0f33251b2581bdcace8a242`  
		Last Modified: Wed, 14 Jul 2021 04:02:29 GMT  
		Size: 44.9 MB (44852175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:4c55d3a5432f13ea7d11d3e16aac59e2f46d61977be2bd63dafbda414030a6f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.9 MB (86925514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d5522f1912d2763e47e403e2f935ed2f813fea46f772222ff8a1e45d8bbc1a`
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
# Tue, 13 Jul 2021 23:20:55 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Tue, 13 Jul 2021 23:21:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 13 Jul 2021 23:21:28 GMT
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
	-	`sha256:b04612a8aa636beb2e3102a0bc60d2aa352f2585b1d443a1afa4573e170f7a84`  
		Last Modified: Tue, 13 Jul 2021 23:34:45 GMT  
		Size: 44.0 MB (44034501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:ba3fd58135d6e2c48697858282af1e664d931ccbcb669118542e425d660a273b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2764090374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55353410361e7df5d834f2896df3984bb093aa3c872a25d4580c5a99df99e02`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:50:59 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 15:57:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:3c8233801d7b9d090726fc4f88542e680df88c6b4bcb6d7ea7dc3e1a08de8fb9`  
		Last Modified: Wed, 14 Jul 2021 17:03:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e6e6c9a18c1433111d9b5108f0e9dea00abf1404c59a64a84588fdb57b7b0`  
		Last Modified: Wed, 14 Jul 2021 17:05:03 GMT  
		Size: 78.6 MB (78640737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-hotspot` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:ee9ef7b76833cfa578e517c6728992e511f9e0464f14b670895b9acd574ab9a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6348208732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d61dc8585bdce7b810ce2f4119189509299566ce5c7f2eeaec3e128b0745f4d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:53:11 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 15:59:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:f503fe00066963e73768cf3ee6026af36fad021a7fa6f29b9cd55bf89b846285`  
		Last Modified: Wed, 14 Jul 2021 17:04:06 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb610bdcdd853dd05dd537e6850aee72ac91885e14249c56b1e282af4f75c53`  
		Last Modified: Wed, 14 Jul 2021 17:05:25 GMT  
		Size: 78.6 MB (78573959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
