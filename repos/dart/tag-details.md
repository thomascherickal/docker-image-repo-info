<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `dart`

-	[`dart:2`](#dart2)
-	[`dart:2-sdk`](#dart2-sdk)
-	[`dart:2.18`](#dart218)
-	[`dart:2.18-sdk`](#dart218-sdk)
-	[`dart:2.18.4`](#dart2184)
-	[`dart:2.18.4-sdk`](#dart2184-sdk)
-	[`dart:2.19.0-255.2.beta`](#dart2190-2552beta)
-	[`dart:2.19.0-255.2.beta-sdk`](#dart2190-2552beta-sdk)
-	[`dart:beta`](#dartbeta)
-	[`dart:beta-sdk`](#dartbeta-sdk)
-	[`dart:latest`](#dartlatest)
-	[`dart:sdk`](#dartsdk)
-	[`dart:stable`](#dartstable)
-	[`dart:stable-sdk`](#dartstable-sdk)

## `dart:2`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2-sdk`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18-sdk`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.18-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.18-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.18.4`

**does not exist** (yet?)

## `dart:2.18.4-sdk`

**does not exist** (yet?)

## `dart:2.19.0-255.2.beta`

```console
$ docker pull dart@sha256:9fa643606ff56e8837b342f4300e360267de82a0a6cc5e5ed265120aa1a5aa30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.0-255.2.beta` - linux; amd64

```console
$ docker pull dart@sha256:d2ae8d5d8aba63bd52daf14c299ced604e997852250825f5ab5229b99af1cbe4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274824754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1077c06d8a7465e9d9f201e04514481562602a97fe2099b067e2c4d8d57ae9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:51 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86419425dac7c6f98e9a39c774dfec5bbe649e1d26b6d91cca60f22cd259873d`  
		Last Modified: Tue, 25 Oct 2022 02:58:37 GMT  
		Size: 196.2 MB (196167283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5626540267d476f7a95f8642dbf6778f3ea3cff91887ff530587f65578fe243d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb2fa7c089641f35c3d038a61ec2392c732f5c341c9be27cdd7033535ac09e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:21:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627cb58a2ff660b7e3b3f1b90c16adbecccdc12c7c81d747f995ee15a3eabaf0`  
		Last Modified: Wed, 26 Oct 2022 05:23:25 GMT  
		Size: 113.8 MB (113806137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:364806a4ebad1b359a02d563be4613a5651aa3789eb8cb8babd13ff66276a1b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.6 MB (191612979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0145e809c991a07d0bac8f2dcda00f3d1e5abab52acb9fd10da431bb1232c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:43:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95dce3609aa52c01109bb4d3589ec66d69385ff6e7384214eb1efe498165ef`  
		Last Modified: Tue, 25 Oct 2022 08:44:20 GMT  
		Size: 115.0 MB (114990503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:2.19.0-255.2.beta-sdk`

```console
$ docker pull dart@sha256:9fa643606ff56e8837b342f4300e360267de82a0a6cc5e5ed265120aa1a5aa30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:2.19.0-255.2.beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d2ae8d5d8aba63bd52daf14c299ced604e997852250825f5ab5229b99af1cbe4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274824754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1077c06d8a7465e9d9f201e04514481562602a97fe2099b067e2c4d8d57ae9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:51 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86419425dac7c6f98e9a39c774dfec5bbe649e1d26b6d91cca60f22cd259873d`  
		Last Modified: Tue, 25 Oct 2022 02:58:37 GMT  
		Size: 196.2 MB (196167283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5626540267d476f7a95f8642dbf6778f3ea3cff91887ff530587f65578fe243d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb2fa7c089641f35c3d038a61ec2392c732f5c341c9be27cdd7033535ac09e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:21:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627cb58a2ff660b7e3b3f1b90c16adbecccdc12c7c81d747f995ee15a3eabaf0`  
		Last Modified: Wed, 26 Oct 2022 05:23:25 GMT  
		Size: 113.8 MB (113806137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:2.19.0-255.2.beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:364806a4ebad1b359a02d563be4613a5651aa3789eb8cb8babd13ff66276a1b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.6 MB (191612979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0145e809c991a07d0bac8f2dcda00f3d1e5abab52acb9fd10da431bb1232c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:43:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95dce3609aa52c01109bb4d3589ec66d69385ff6e7384214eb1efe498165ef`  
		Last Modified: Tue, 25 Oct 2022 08:44:20 GMT  
		Size: 115.0 MB (114990503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta`

```console
$ docker pull dart@sha256:9fa643606ff56e8837b342f4300e360267de82a0a6cc5e5ed265120aa1a5aa30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta` - linux; amd64

```console
$ docker pull dart@sha256:d2ae8d5d8aba63bd52daf14c299ced604e997852250825f5ab5229b99af1cbe4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274824754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1077c06d8a7465e9d9f201e04514481562602a97fe2099b067e2c4d8d57ae9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:51 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86419425dac7c6f98e9a39c774dfec5bbe649e1d26b6d91cca60f22cd259873d`  
		Last Modified: Tue, 25 Oct 2022 02:58:37 GMT  
		Size: 196.2 MB (196167283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm variant v7

```console
$ docker pull dart@sha256:5626540267d476f7a95f8642dbf6778f3ea3cff91887ff530587f65578fe243d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb2fa7c089641f35c3d038a61ec2392c732f5c341c9be27cdd7033535ac09e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:21:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627cb58a2ff660b7e3b3f1b90c16adbecccdc12c7c81d747f995ee15a3eabaf0`  
		Last Modified: Wed, 26 Oct 2022 05:23:25 GMT  
		Size: 113.8 MB (113806137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:364806a4ebad1b359a02d563be4613a5651aa3789eb8cb8babd13ff66276a1b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.6 MB (191612979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0145e809c991a07d0bac8f2dcda00f3d1e5abab52acb9fd10da431bb1232c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:43:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95dce3609aa52c01109bb4d3589ec66d69385ff6e7384214eb1efe498165ef`  
		Last Modified: Tue, 25 Oct 2022 08:44:20 GMT  
		Size: 115.0 MB (114990503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:beta-sdk`

```console
$ docker pull dart@sha256:9fa643606ff56e8837b342f4300e360267de82a0a6cc5e5ed265120aa1a5aa30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:beta-sdk` - linux; amd64

```console
$ docker pull dart@sha256:d2ae8d5d8aba63bd52daf14c299ced604e997852250825f5ab5229b99af1cbe4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.8 MB (274824754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1077c06d8a7465e9d9f201e04514481562602a97fe2099b067e2c4d8d57ae9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:51 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86419425dac7c6f98e9a39c774dfec5bbe649e1d26b6d91cca60f22cd259873d`  
		Last Modified: Tue, 25 Oct 2022 02:58:37 GMT  
		Size: 196.2 MB (196167283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:5626540267d476f7a95f8642dbf6778f3ea3cff91887ff530587f65578fe243d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182630787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79eb2fa7c089641f35c3d038a61ec2392c732f5c341c9be27cdd7033535ac09e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:21:15 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627cb58a2ff660b7e3b3f1b90c16adbecccdc12c7c81d747f995ee15a3eabaf0`  
		Last Modified: Wed, 26 Oct 2022 05:23:25 GMT  
		Size: 113.8 MB (113806137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:beta-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:364806a4ebad1b359a02d563be4613a5651aa3789eb8cb8babd13ff66276a1b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.6 MB (191612979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f0145e809c991a07d0bac8f2dcda00f3d1e5abab52acb9fd10da431bb1232c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:43:02 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=1f7f7ca69fde326ec7b67e2467581e174feab05d8b565742af70a33eb4d9ee04;             SDK_ARCH="x64";;         armhf)             DART_SHA256=efb811288c7f5f1ef52284a85d673ef023fa34c9ff0845578425b4d72d74fe64;             SDK_ARCH="arm";;         arm64)             DART_SHA256=8fd51694cc0d94fd393669a8ada893ca76e4097eb2f32fc3a95ceb8a4204e437;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/beta/release/2.19.0-255.2.beta/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95dce3609aa52c01109bb4d3589ec66d69385ff6e7384214eb1efe498165ef`  
		Last Modified: Tue, 25 Oct 2022 08:44:20 GMT  
		Size: 115.0 MB (114990503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:latest`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:latest` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:latest` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:sdk`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:sdk` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `dart:stable-sdk`

```console
$ docker pull dart@sha256:6bc2a4a220e08b60d8f52ad3c085f527e00ce334ac19e365b40fab9d4256e8e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `dart:stable-sdk` - linux; amd64

```console
$ docker pull dart@sha256:6e39250ea9476f1bb1e9a95e3f63f28efd927e300cf512074bb0daf0840602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (271983100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daacd76829936449a97427b70266dd6adf01a1e00a5784e0d4ca75d6b8254449`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:56:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:56:20 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 02:56:20 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 02:56:20 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 02:56:20 GMT
WORKDIR /root
# Tue, 25 Oct 2022 02:56:32 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985265eb3a3bc7dc12be38e2397bdf2f5fbe7d911aa7de110b6fa45fed49c4a`  
		Last Modified: Tue, 25 Oct 2022 02:57:19 GMT  
		Size: 45.1 MB (45075394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fb1ddbabe5d7223af8c15bce88526e37f6e4b66725898a9c6cd1bf490e38f8`  
		Last Modified: Tue, 25 Oct 2022 02:57:12 GMT  
		Size: 2.2 MB (2162039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662567cc28bc5787a0ac2607b6670ec02b9b18d07dec4a205b235ffdbb589f34`  
		Last Modified: Tue, 25 Oct 2022 02:57:40 GMT  
		Size: 193.3 MB (193325629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm variant v7

```console
$ docker pull dart@sha256:b1381922247ecd7dcf5c731858ac000208dbd21299eb8d5dd0c469ed8445df3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.6 MB (180603013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d683c5ad9eeb829b3f6048dcd26278c2caf97ddff20690eaf64f891909f68799`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 05:20:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 05:20:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Wed, 26 Oct 2022 05:20:42 GMT
ENV DART_SDK=/usr/lib/dart
# Wed, 26 Oct 2022 05:20:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 05:20:43 GMT
WORKDIR /root
# Wed, 26 Oct 2022 05:20:53 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cbc3347d739c6071195c82790554c65151674e44a4f05eee5d340d664a079`  
		Last Modified: Wed, 26 Oct 2022 05:22:11 GMT  
		Size: 41.0 MB (40956844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72687a57d437ab9e926ef050b8e26adab5ea1ac0de3551a93cc998ea043a5d81`  
		Last Modified: Wed, 26 Oct 2022 05:22:04 GMT  
		Size: 1.3 MB (1288513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94310e55ce5f50fa51a3f820ee01cf910badc7526cb1998081df8a2f6de65d9`  
		Last Modified: Wed, 26 Oct 2022 05:22:24 GMT  
		Size: 111.8 MB (111778363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `dart:stable-sdk` - linux; arm64 variant v8

```console
$ docker pull dart@sha256:904e8cb727cfe862c497f6144fa639f61e7de286cbb6e38c8f3232fccc6251c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189562109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d12451eacad86dcaa4911145b778ba90a63cf38d1722af693229a5bccbfbc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:42:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends         ca-certificates         curl         dnsutils         git         openssh-client         unzip     ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:42:42 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             TRIPLET="x86_64-linux-gnu" ;             FILES="/lib64/ld-linux-x86-64.so.2" ;;         armhf)             TRIPLET="arm-linux-gnueabihf" ;             FILES="/lib/ld-linux-armhf.so.3                 /lib/arm-linux-gnueabihf/ld-linux-armhf.so.3";;         arm64)             TRIPLET="aarch64-linux-gnu" ;             FILES="/lib/ld-linux-aarch64.so.1                 /lib/aarch64-linux-gnu/ld-linux-aarch64.so.1" ;;         *)             echo "Unsupported architecture" ;             exit 5;;     esac;     FILES="$FILES         /etc/nsswitch.conf         /etc/ssl/certs         /usr/share/ca-certificates         /lib/$TRIPLET/libc.so.6         /lib/$TRIPLET/libdl.so.2         /lib/$TRIPLET/libm.so.6         /lib/$TRIPLET/libnss_dns.so.2         /lib/$TRIPLET/libpthread.so.0         /lib/$TRIPLET/libresolv.so.2         /lib/$TRIPLET/librt.so.1";     for f in $FILES; do         dir=$(dirname "$f");         mkdir -p "/runtime$dir";         cp --archive --link --dereference --no-target-directory "$f" "/runtime$f";     done
# Tue, 25 Oct 2022 08:42:42 GMT
ENV DART_SDK=/usr/lib/dart
# Tue, 25 Oct 2022 08:42:42 GMT
ENV PATH=/usr/lib/dart/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:42:42 GMT
WORKDIR /root
# Tue, 25 Oct 2022 08:42:48 GMT
RUN set -eux;     case "$(dpkg --print-architecture)" in         amd64)             DART_SHA256=77ffe06da481ce420463349d339998dcb122f8c7a857ab96acd35a4652d47e3d;             SDK_ARCH="x64";;         armhf)             DART_SHA256=0e5f0f3bf591bbc0a8561171ebfdba3a2da566600d4fcdd6bd6a614201c304e0;             SDK_ARCH="arm";;         arm64)             DART_SHA256=e7ddd9e8c7160b72f61af674e8715f01df4ad445a92685cf86f7b0701fb44027;             SDK_ARCH="arm64";;     esac;     SDK="dartsdk-linux-${SDK_ARCH}-release.zip";     BASEURL="https://storage.googleapis.com/dart-archive/channels";     URL="$BASEURL/stable/release/2.18.3/sdk/$SDK";     echo "SDK: $URL" >> dart_setup.log ;     curl -fLO "$URL";     echo "$DART_SHA256 *$SDK"         | sha256sum --check --status --strict -;     unzip "$SDK" && mv dart-sdk "$DART_SDK" && rm "$SDK"         && chmod 755 "$DART_SDK" && chmod 755 "$DART_SDK/bin";
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf5a788deb256c38f906c16ef48daec5c77a424abb1c72dc7c9f38ad3627bf7`  
		Last Modified: Tue, 25 Oct 2022 08:43:27 GMT  
		Size: 45.0 MB (44996382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66c9297aeaf200264e172369195971c5f26cc119206a149b679556c8f468c67`  
		Last Modified: Tue, 25 Oct 2022 08:43:22 GMT  
		Size: 1.6 MB (1562184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bccb61bde83cf04316456560430086d0457544309cddb00adc5a601fa50ae5`  
		Last Modified: Tue, 25 Oct 2022 08:43:35 GMT  
		Size: 112.9 MB (112939633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
