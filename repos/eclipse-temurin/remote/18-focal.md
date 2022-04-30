## `eclipse-temurin:18-focal`

```console
$ docker pull eclipse-temurin@sha256:b8d70d563fd7ee208de070ece837160a4b4147c584daafdeee331e10a2710243
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:18-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:3b525c809c452778fc104b975d9560d8c2544d241d036504c503df9ce81e93cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241770122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de8309a91d98b7748c9710c4b6e0378fb3fc0d12daa647fe804fd665ddfb85a1`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:04:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 02:05:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:06:30 GMT
ENV JAVA_VERSION=jdk-18+36
# Fri, 22 Apr 2022 02:06:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='e696d2b5995ae008b6ee7392d73ace13c36460a5e9600740c40e094079a62d28';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_aarch64_linux_hotspot_18_36.tar.gz';          ;;        armhf|arm)          ESUM='4cb2e1fe9a14a990ad0dc8f3afcd9c1b37a8d7750754c3a1e72665ef6beb300f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_arm_linux_hotspot_18_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='90790055be8147103a4a9b6a6545d42d7c5eb5616901b660c8ada68c7d067956';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_ppc64le_linux_hotspot_18_36.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='e711965a3c482a63d0116bcb0f3c1d06b84171c4be1995f3ac9f139d316fe149';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_s390x_linux_hotspot_18_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='82d67983f92f16b5fb57176fa4c228e44ecc6f671b3c3523140fba7fb904dceb';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 02:06:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 02:06:50 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 02:06:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba7eb4b0706bdc82016e578b506e90d02ab8407a4ac8ed832da3eb310a8494`  
		Last Modified: Fri, 22 Apr 2022 02:09:43 GMT  
		Size: 19.8 MB (19771621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33245e75cce12da72da2411775e6cd7054f60e30ed0a50300212a23b8f4066da`  
		Last Modified: Fri, 22 Apr 2022 02:11:12 GMT  
		Size: 193.4 MB (193432343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5383940554afb16e3ae87d655848965808256d09f52eefb2883f442b78099b1e`  
		Last Modified: Fri, 22 Apr 2022 02:10:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-focal` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:9d061ec094b533b129fdee5135e98f09bec8213eef816d381c42f4f562445bd7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233860584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80af6e17b972ae907daaee26aef06170f4e48b83bcd52e9ee466245238d099ee`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:56:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:59:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:00:58 GMT
ENV JAVA_VERSION=jdk-18+36
# Sat, 30 Apr 2022 00:01:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='e696d2b5995ae008b6ee7392d73ace13c36460a5e9600740c40e094079a62d28';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_aarch64_linux_hotspot_18_36.tar.gz';          ;;        armhf|arm)          ESUM='4cb2e1fe9a14a990ad0dc8f3afcd9c1b37a8d7750754c3a1e72665ef6beb300f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_arm_linux_hotspot_18_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='90790055be8147103a4a9b6a6545d42d7c5eb5616901b660c8ada68c7d067956';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_ppc64le_linux_hotspot_18_36.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='e711965a3c482a63d0116bcb0f3c1d06b84171c4be1995f3ac9f139d316fe149';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_s390x_linux_hotspot_18_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='82d67983f92f16b5fb57176fa4c228e44ecc6f671b3c3523140fba7fb904dceb';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:01:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:01:26 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 30 Apr 2022 00:01:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362c401df4a70d7113d00849e1040eba62e153171d43aeb505cdfe041e13b30f`  
		Last Modified: Sat, 30 Apr 2022 00:07:40 GMT  
		Size: 19.2 MB (19195606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c55469cbdca8962541a7197d645897d8671bde1cd57834d88698b6d3baf7c8`  
		Last Modified: Sat, 30 Apr 2022 00:10:51 GMT  
		Size: 190.6 MB (190591168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b53786a055d98c72f2c2a4f95e1cbfc3ab48efefe7874114e0e08011ad1149a`  
		Last Modified: Sat, 30 Apr 2022 00:09:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:5c384447631f8bf3bb53cdcf6150483c2059bf74c7e1b328a8369434eb34896e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.0 MB (239968969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b69182faf15865c0f502597c9479224bb2060b4df9960bc8e51d8209b40124c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:31:40 GMT
ENV JAVA_VERSION=jdk-18+36
# Fri, 29 Apr 2022 23:31:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='e696d2b5995ae008b6ee7392d73ace13c36460a5e9600740c40e094079a62d28';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_aarch64_linux_hotspot_18_36.tar.gz';          ;;        armhf|arm)          ESUM='4cb2e1fe9a14a990ad0dc8f3afcd9c1b37a8d7750754c3a1e72665ef6beb300f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_arm_linux_hotspot_18_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='90790055be8147103a4a9b6a6545d42d7c5eb5616901b660c8ada68c7d067956';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_ppc64le_linux_hotspot_18_36.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='e711965a3c482a63d0116bcb0f3c1d06b84171c4be1995f3ac9f139d316fe149';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_s390x_linux_hotspot_18_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='82d67983f92f16b5fb57176fa4c228e44ecc6f671b3c3523140fba7fb904dceb';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:31:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:31:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 29 Apr 2022 23:31:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a402fc50caa18dd54616de2d8887d0ddfcb2a6b725894ed6c23004fa8e2090c`  
		Last Modified: Fri, 29 Apr 2022 23:36:31 GMT  
		Size: 192.3 MB (192300100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1669e88c182480f86f71b94030c98b89ecb67fff97df739978d617044e04fb76`  
		Last Modified: Fri, 29 Apr 2022 23:36:13 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:0ceba8c3d48e6061e254ee668ba98f5877164693c4fe3e6dd2f209acc00a690c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.8 MB (247814667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4513d0779d09ab2fef6f065d61a5adca647a1b5829bb0f061e74504637707297`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:45:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 22 Apr 2022 09:51:59 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:54:42 GMT
ENV JAVA_VERSION=jdk-18+36
# Fri, 22 Apr 2022 09:55:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='e696d2b5995ae008b6ee7392d73ace13c36460a5e9600740c40e094079a62d28';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_aarch64_linux_hotspot_18_36.tar.gz';          ;;        armhf|arm)          ESUM='4cb2e1fe9a14a990ad0dc8f3afcd9c1b37a8d7750754c3a1e72665ef6beb300f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_arm_linux_hotspot_18_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='90790055be8147103a4a9b6a6545d42d7c5eb5616901b660c8ada68c7d067956';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_ppc64le_linux_hotspot_18_36.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='e711965a3c482a63d0116bcb0f3c1d06b84171c4be1995f3ac9f139d316fe149';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_s390x_linux_hotspot_18_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='82d67983f92f16b5fb57176fa4c228e44ecc6f671b3c3523140fba7fb904dceb';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 22 Apr 2022 09:55:16 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 09:55:29 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 22 Apr 2022 09:55:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b871f7e17903642296f4fb5f218d67a797860ca4d97df5f5cd9f44cc0e39ed8a`  
		Last Modified: Fri, 22 Apr 2022 10:00:23 GMT  
		Size: 21.7 MB (21690280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84676354a21f841e033b6418bb9e9df7a6e7203c3421a295bfa90212a4167c4`  
		Last Modified: Fri, 22 Apr 2022 10:02:21 GMT  
		Size: 192.8 MB (192833851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab238e6929beca9b3f9df6bc45896acc1a35dd57c7ccc7c9ee7e04a3fffa4b4`  
		Last Modified: Fri, 22 Apr 2022 10:02:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-focal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:62eac17e76b9b9cae833b6b7d866cfc2be4b48f3dd545445fc8da8b7bc03f951
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.7 MB (227715429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2f04c83eb2c2a4cfe63759ed018c3ecd53f6016075608a82a1c2125999a063`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:22:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:23:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:24:15 GMT
ENV JAVA_VERSION=jdk-18+36
# Fri, 29 Apr 2022 23:24:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='e696d2b5995ae008b6ee7392d73ace13c36460a5e9600740c40e094079a62d28';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_aarch64_linux_hotspot_18_36.tar.gz';          ;;        armhf|arm)          ESUM='4cb2e1fe9a14a990ad0dc8f3afcd9c1b37a8d7750754c3a1e72665ef6beb300f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_arm_linux_hotspot_18_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='90790055be8147103a4a9b6a6545d42d7c5eb5616901b660c8ada68c7d067956';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_ppc64le_linux_hotspot_18_36.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='e711965a3c482a63d0116bcb0f3c1d06b84171c4be1995f3ac9f139d316fe149';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_s390x_linux_hotspot_18_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='82d67983f92f16b5fb57176fa4c228e44ecc6f671b3c3523140fba7fb904dceb';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_linux_hotspot_18_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 29 Apr 2022 23:24:27 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Apr 2022 23:24:27 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 29 Apr 2022 23:24:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8061a8e3bb73503261725cfaf9256d8c5dc9ee8d357d1e40a4d6578ad8263162`  
		Last Modified: Fri, 29 Apr 2022 23:25:57 GMT  
		Size: 19.2 MB (19235277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6572443b8538e0a9a1f0b0e0ac60444b6815b2638a4ca8b84ee050be6dfcf47`  
		Last Modified: Fri, 29 Apr 2022 23:26:37 GMT  
		Size: 181.4 MB (181414575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14a0671a04e774b17a66cf2ab9bec123aa25c0d01707d71c472e448fc16c7c7`  
		Last Modified: Fri, 29 Apr 2022 23:26:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
