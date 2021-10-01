## `eclipse-temurin:11-jdk`

```console
$ docker pull eclipse-temurin@sha256:de2abd6c3c0e2a9b701c31f59c3bbfa720f5933d62aa540280e1e02aa8c1779f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `eclipse-temurin:11-jdk` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:f0ee0ef496b2828e0f47a9d667b439b7f14457bda2f91868fa4810d7e41c607e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.4 MB (238415490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4043fe7c4d087a134a27aa448101191e188809a6bdde779bc9649ee11701cb2`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:26:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 03:31:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Sep 2021 23:20:01 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Thu, 16 Sep 2021 19:24:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Sep 2021 19:24:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Sep 2021 19:24:11 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 16 Sep 2021 19:24:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df1ad422e5a232e54d515fb2475eee78b57b25d905611bbceb50f364c0150c`  
		Last Modified: Tue, 31 Aug 2021 03:33:27 GMT  
		Size: 16.0 MB (16032853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfcc24a13503106691620bc7b42f463fcc6c368a2e1d606469551f9596417c1`  
		Last Modified: Thu, 16 Sep 2021 19:25:51 GMT  
		Size: 193.8 MB (193812402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b577d861249d9950144e676aee0d585b6de5656b3da69f5297dd50aabe6b0695`  
		Last Modified: Thu, 16 Sep 2021 19:25:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:47dca4d665a2650be3a15fa225d2d6715331fcc141daa6da379aaca2eaeec17f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220676497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ee84c7cb4ee6096e3911971f9b16276f4ad455dbd1ef1e62ec1c9ed9e5df29b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:51:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 22 Sep 2021 20:40:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Sep 2021 20:40:48 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 22 Sep 2021 20:41:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Sep 2021 20:41:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Sep 2021 20:41:12 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 22 Sep 2021 20:41:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38ad2952682521263306c30b66265ca7508f3287f2cfd9b8cb935f2a0be95fd`  
		Last Modified: Wed, 22 Sep 2021 20:43:33 GMT  
		Size: 14.9 MB (14902107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6868e9a5cabfcc6ab83f07ac4d5cf1142318bf1ff95e997b5422618779f3a005`  
		Last Modified: Wed, 22 Sep 2021 20:44:31 GMT  
		Size: 181.7 MB (181705407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7438a9d4145770dc3a2539f342419d3035e84cc8f6f536c9973a65072241a6b`  
		Last Modified: Wed, 22 Sep 2021 20:43:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:f2dd87b97f6449c2cdc8f8e5095572a8d77fa79956537abad51b454e41031ecb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.6 MB (233572598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8234ab8f892d769d4943d77f5d6832f4656cd60839c5c3b946c0a5a2fd4a7d98`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:59:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:25:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 13 Sep 2021 17:40:27 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Thu, 16 Sep 2021 19:40:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Sep 2021 19:40:13 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Sep 2021 19:40:14 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 16 Sep 2021 19:40:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1d8585069a0a852415434548e9df1c5314c6721293171b6ed14a607e76247d`  
		Last Modified: Tue, 31 Aug 2021 02:28:37 GMT  
		Size: 15.9 MB (15897608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7396d93b3227f0206b19b7a193f14851f7b6676867559d49e8b8ecee5599464`  
		Last Modified: Thu, 16 Sep 2021 19:42:59 GMT  
		Size: 190.5 MB (190501729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacc4bedb17c1e65e68a0651792f318ab904a0899d1717a00bd73328ad9436b7`  
		Last Modified: Thu, 16 Sep 2021 19:42:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:00cb74ca670e8245b9c6cb90a21b47aa75335417df90a3ef00481be0b8813bee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226186311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81b087e6247c5782660028a583bb73430e003c8dff641e6425b98fcb36ada40c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 05:45:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 13 Sep 2021 20:42:15 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Thu, 16 Sep 2021 19:17:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Sep 2021 19:17:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Sep 2021 19:18:07 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 16 Sep 2021 19:18:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22897a482fa0e59d16e7302ee8b24736e577f4a14e821586507f289c961d84c9`  
		Last Modified: Tue, 31 Aug 2021 05:51:33 GMT  
		Size: 17.2 MB (17207875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6626ae7a987929b719f8f5a582ef37544f773f601185ce9d0afe52026386852`  
		Last Modified: Thu, 16 Sep 2021 19:23:09 GMT  
		Size: 175.7 MB (175686484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ed813347fbeabf99e4667e389e968f762e185414498bcf51974984f8685a84`  
		Last Modified: Thu, 16 Sep 2021 19:22:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:5534717d976afc3188590d44132d6aa8a9562837e9995aafaf4e3c2d0a58e33d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.6 MB (211588962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc991b991b9b8280ef9234651369145e9959cfb13217d8bd0882de3148ca960e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:00:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 02:45:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:45:11 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Fri, 01 Oct 2021 02:45:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='105bdc12fcd54c551e8e8ac96bc82412467244c32063689c41cee29ceb7452a2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.12_7.tar.gz';          ;;        armhf|arm)          ESUM='85929246a9d60ed90e2385ea3f4857798c77019c5100f00189c1dd0a093abea7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.12_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='234a9bafe029ea6cab5d46f9617b5d016a29faa187a42081d0e066f23647b7e5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.12_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='99c1c61e9d67b01a649687189e5a00f89a2371dc1bfed06bb078d127edfa7995';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.12_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8770f600fc3b89bf331213c7aa21f8eedd9ca5d96036d1cd48cb2748a3dbefd2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 02:45:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 02:45:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 01 Oct 2021 02:45:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ea6869b37d6809b4bdfbfc83b247246d2b56380b1c1f285e93eeabdda12def`  
		Last Modified: Fri, 01 Oct 2021 02:47:18 GMT  
		Size: 15.7 MB (15739143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23e574391ab9e0facf4a6804549a0887f931b21165c9f8e32dcb93b00cd1985`  
		Last Modified: Fri, 01 Oct 2021 02:47:27 GMT  
		Size: 168.7 MB (168726748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec18cee38f6c49dd9f10d014d4e5264840f82b9d93d3b2523d0a088083d445b9`  
		Last Modified: Fri, 01 Oct 2021 02:47:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - windows version 10.0.17763.2183; amd64

```console
$ docker pull eclipse-temurin@sha256:8954b4510ff8c6531fe55ed435264f5829dd5219930fd3cd999e5210b319f61b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3052572665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2697c8d816bd7fa2c8eebc8b3721fe42a34d004d432d14561d9343c9f142ba03`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 16:25:52 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 15 Sep 2021 16:27:15 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ;     Write-Host ('Verifying sha256 (80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Sep 2021 16:28:00 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Sep 2021 16:28:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce788feb9aeea314f2ff314f767f80f5b8c72bed0378fe10224022eb94d418a4`  
		Last Modified: Wed, 15 Sep 2021 16:44:29 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9063ef0b0d47b843faeaa1cb27aa693f2948ff9abda9f89d67d0c91f5ffa0c0c`  
		Last Modified: Wed, 15 Sep 2021 16:50:51 GMT  
		Size: 365.5 MB (365548642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72192107ea9ec1b2a0fd6ad29fc640fb556c6266b7a3c2be7d4046aa8a2478bb`  
		Last Modified: Wed, 15 Sep 2021 16:44:30 GMT  
		Size: 322.1 KB (322108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3811107e84d31c6bdaefe2ae4cae3e722adb9aad23c6256b96d9e084aa16a9`  
		Last Modified: Wed, 15 Sep 2021 16:44:29 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk` - windows version 10.0.14393.4651; amd64

```console
$ docker pull eclipse-temurin@sha256:40adbc50c545b5fc4e24409e9f9be49670eaeb2cf21e6580060f8c1b66126d8a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6637130324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cfb8feff5c23383ed889b2735d2ee885a06381ecf02127bcb4b3d34100f834`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 16:28:20 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 15 Sep 2021 16:29:45 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Sep 2021 16:30:38 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Sep 2021 16:30:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bad1262ba6d2ce354dd77660b54caba20d1b11cc7f16b064df1ea6fb2716467`  
		Last Modified: Wed, 15 Sep 2021 16:51:13 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc124491808397e9345a1fba2e688c02749b08ab0f1830526a987751f432e588`  
		Last Modified: Wed, 15 Sep 2021 16:51:34 GMT  
		Size: 365.5 MB (365489510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b699250a6b2dc1b1afc2ad81e45fdb8addc39f5c6ff4dd4975529565949bf54`  
		Last Modified: Wed, 15 Sep 2021 16:51:09 GMT  
		Size: 308.7 KB (308675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135a93ce7e50e4c637cc7974d4b802241a8e34b3cb409dfb3d38705a3d50333`  
		Last Modified: Wed, 15 Sep 2021 16:51:09 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
