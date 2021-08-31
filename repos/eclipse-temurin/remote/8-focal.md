## `eclipse-temurin:8-focal`

```console
$ docker pull eclipse-temurin@sha256:764077aa435b3a60a4220c438b807ad2492166e35fed7685d502ea2eb383e6a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:3e4773d53b15c0b371e543798ba7e2858c74c2291639ab4aa7506df5fdca5277
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151895125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ec5430c545405b33f346d5d175442f9b283ca5a30aa80e2cef26c00fd817d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:26:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 03:30:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl binutils ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:30:53 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Tue, 31 Aug 2021 03:30:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f287cdc2a688c2df247ea0d8bfe2863645b73848e4e5c35b02a8a3d2d6b69551';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u302b08.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c2940f3772d4467a818a0221e80c2c720b6d427a886aaed37262e451ddbb0a56';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u302b08.tar.gz';          ;;        amd64|x86_64)          ESUM='cc13f274becf9dd5517b6be583632819dfd4dd81e524b5c1b4f406bdaf0e063a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u302b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 03:30:59 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 03:31:00 GMT
RUN echo Verifying install ...     && echo   javac -version && javac -version     && echo   java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f9d1409456f073be8f4584cba31886fecf3daccb3e3b04ca5972fa1ebef37`  
		Last Modified: Tue, 31 Aug 2021 03:33:05 GMT  
		Size: 19.8 MB (19775633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d10cc096367c2f451415aea348e8e5f78f63cadb5470aae24d78ddb0e3034`  
		Last Modified: Tue, 31 Aug 2021 03:33:11 GMT  
		Size: 103.5 MB (103549258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28bcdae83cf715dfcc09bc38fc0d077403331c217803881646500b30e112491`  
		Last Modified: Tue, 31 Aug 2021 03:33:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:541963730293cc6a5dfaa1c12b5907b865116bae2016c3bf0e7bd9535adaff6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150374631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4797cc0d4ed78ddfc7d4c8c5f3b622009f4d712ad0161acd90c4d04c36bb1c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:44 GMT
ADD file:cec21619ecbd37b4cf8da15153b8957a343cd25c6f714e3ac3969b6003704a58 in / 
# Tue, 31 Aug 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 01:59:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:25:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl binutils ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:25:00 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Tue, 31 Aug 2021 02:25:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f287cdc2a688c2df247ea0d8bfe2863645b73848e4e5c35b02a8a3d2d6b69551';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u302b08.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c2940f3772d4467a818a0221e80c2c720b6d427a886aaed37262e451ddbb0a56';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u302b08.tar.gz';          ;;        amd64|x86_64)          ESUM='cc13f274becf9dd5517b6be583632819dfd4dd81e524b5c1b4f406bdaf0e063a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u302b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:25:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:25:07 GMT
RUN echo Verifying install ...     && echo   javac -version && javac -version     && echo   java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:ab2d02b1ec420fdb84c9f52abda403b6aef20f5de904a2ecda5ae4f5cd6e4d46`  
		Last Modified: Tue, 31 Aug 2021 01:42:34 GMT  
		Size: 27.2 MB (27173099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd255873a8de7ec037b5b3f6a87d4685e3cce3797739ca6d30f624fb9685032`  
		Last Modified: Tue, 31 Aug 2021 02:28:09 GMT  
		Size: 20.5 MB (20499326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b845a6187e8306b22414746f772f6b2db77f7fb2708e5fa2d1139ccc835b195`  
		Last Modified: Tue, 31 Aug 2021 02:28:17 GMT  
		Size: 102.7 MB (102702046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713243eaded58349c52e3db66b83828b7485d254cff3a3be54b92d03f2a7a4d3`  
		Last Modified: Tue, 31 Aug 2021 02:28:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:e56fcd9f8905492a048a870c365b9af38574af29d7a77de7b8a3e698fbe721a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156050019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9855ab33a276945b0acababf6eedabfee6d32ea2baf76eba78d57072a89a926`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 05:42:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl binutils ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 05:42:56 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Tue, 31 Aug 2021 05:43:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f287cdc2a688c2df247ea0d8bfe2863645b73848e4e5c35b02a8a3d2d6b69551';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_hotspot_8u302b08.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='c2940f3772d4467a818a0221e80c2c720b6d427a886aaed37262e451ddbb0a56';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u302b08.tar.gz';          ;;        amd64|x86_64)          ESUM='cc13f274becf9dd5517b6be583632819dfd4dd81e524b5c1b4f406bdaf0e063a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u302b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 05:43:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 05:43:24 GMT
RUN echo Verifying install ...     && echo   javac -version && javac -version     && echo   java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3e610dbb46263ed8dbbc570c6012c3baefb0764e29536e7b1a5ef2186a4491`  
		Last Modified: Tue, 31 Aug 2021 05:51:04 GMT  
		Size: 21.7 MB (21686033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06b7bebc629c64179acd23e398349393c32d518d038f8aa7d715cacd203d3f9`  
		Last Modified: Tue, 31 Aug 2021 05:51:12 GMT  
		Size: 101.1 MB (101072036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283fac0df86a02c2164e4145d0f860f3d2d83bd455a37fa22fe6a66eee8f7de3`  
		Last Modified: Tue, 31 Aug 2021 05:50:59 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
